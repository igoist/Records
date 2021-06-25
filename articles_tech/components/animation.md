过渡动画封装实现


分享会中提到的几个问题，在这里整理一下：

* 如何去便利地观察动画相关 class 类命

当时有同学提到去调整 duration，可如果是自己项目的代码，那本身已经是知道到底是哪个 class 在产生影响，前后是矛盾的。

除了当时说的录屏大法，用 Devtools 自带的 Animations 思路是对的，不过当时太紧张，俺把之前学过的也给忘了，一直傻傻地在点快照。

这里继续以当时那个 Antd 中的 Modal 为例子，为了观察 class，先打开 Animations 选项卡，将 speed(100% 25% 10% 那一栏) 设置为 10%，并点击左侧 Pause all。

接着先去点击 Antd 网页中任意一个 Open Modal 按钮，然后重新点击刚才那个 Pause all(此时是蓝色按钮，hover 后可见 Resume all)，这时你可以看到动画开始执行，弹窗在慢慢地打开来，

那么再点一次暂停(就是那个 Pause all)，砸瓦鲁多，动画停止。

后面的事还用俺啰嗦吗，需要观察的 class 就在 Elements 选项卡中对应的元素上。

(如视频中最后，当相关类存在，在 Styles 这一栏底部盒模型的上方，展示了 keyframe 的具体属性值)


* 关于通过使用 setTimeout 定时器来替代 transitionend、animationend，实现类似动画效果是否可行

玩一下当然可以，最早在俺晓得有 transitionend、animationend 这俩 dom 原生事件之前，俺就是那么做的。

但是有经验一点的同学应该知道，动画的渲染进程有可能被阻塞。

换句话说，你本来预设了一个动画 0.3s 结束，你想弄个 3 倍时长的定时器设个 0.9s 总够了吧(战术后仰)，但是弄不好因为渲染进程被阻塞，然后某次动画刚刚刚刚好在 0.91s 才结束，于是就会得到非预期的结果。


* 如果想让一个元素的当前动画过程暂停，并且在此基础上继续执行下一个动画，怎么实现

对 animation 陌生的同学，如果有把这个问题搞明白的欲望，那么首先得先去翻翻 MDN 对于 animation-play-state、animation-fill-mode 等动画相关属性的介绍。

当需要淡入的元素添加类 xx-fade-enter, xx-fade-enter-active 后，属性 animation-play-state 的值为 running，如果对这个元素添加 animation-play-state: paused，动画自然也会暂停。

仍然参考 Modal，这里假定动画开始时为 0%，动画结束时为 100%，以淡入动画 50% 进度为例，在这个时间点用户进行了点击，触发了淡出动画，说实话，俺暂时想不到好的处理办法。

理想情况当然应该是淡入已经从 0% 完成到 50%，此时淡出从 50% 返回到 0%，然而浏览器并不允许啊！

像 antd 的 Modal，当淡入过程进行到 50%，此时去触发弹窗关闭，会像下面视频中那样，将类 ant-fade-enter、ant-fade-enter-active 移除，

并添加 ant-fade-leave、ant-fade-leave-active，淡入时的 animation-name antZoomIn 被更新成了 antZoomOut，于是 ant-modal 这个 dom 元素也被更新至了 antZoomOut 中的初始状态：'transform: scale(1); opacity: 1;'






实际上如果自己从零开始实现这类过渡动画，会遇到不少各种各种的问题，就比方俺早期，写了非常多重复的代码，最后发现其实可以重新封装成下面这样两部分，js 和 css

interface ETAnimationConfigType {
  el: any;
  name?: string;
  isEnter?: boolean;
  callback?: () => any;
}

/**
 * el
 * name: string    'fade' | 'slide-up'
 * isEnter?: boolean
 * callback?: () => {}
 */
export const ETAnimation = (config: ETAnimationConfigType) => {
  // tmp prefix
  const prefix = 'et';

  const { el, name, isEnter = false, callback } = config;

  const suffix = isEnter ? 'enter' : 'leave';

  const pf = `${prefix}-${name}-${suffix}`;

  // 避免冲突
  if (hasClass(`${pf}`, el)) {
    return;
  }

  const handleFade = () => {
    el.classList.remove(`${pf}`);
    el.classList.remove(`${pf}-active`);
    el.removeEventListener('animationend', handleFade);

    if (callback) {
      callback();
    }
  };

  el.addEventListener('animationend', handleFade);
  el.classList.add(`${pf}`);
  el.classList.add(`${pf}-active`);
};

export const ETFade = (config: ETAnimationConfigType) => {
  config.name = 'fade';

  ETAnimation(config);
};

export const ETZoom = (config: ETAnimationConfigType) => {
  config.name = 'zoom';

  ETAnimation(config);
};


// 注：$P 可自由定于，偷懒的话直接定义成
$P: 'et';

// mixin
@mixin ETAnimationMixin($pf) {
  .#{$pf}-enter,
  .#{$pf}-leave {
    animation-duration: 0.3s;
    animation-fill-mode: both;
    animation-play-state: paused;
  }

  .#{$pf}-enter.#{$pf}-enter-active {
    animation-play-state: running;
  }

  .#{$pf}-leave.#{$pf}-leave-active {
    animation-play-state: running;
    pointer-events: none;
  }

  .#{$pf}-enter,
  .#{$pf}-leave {
    animation-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1);
  }

  .#{$pf}-enter {
    opacity: 0;
  }
}

// _animation
$PF: $P + '-fade';

@include ETAnimationMixin($PF);

.#{$PF}-enter.#{$PF}-enter-active {
  animation-name: ETFadeEnter;
}

.#{$PF}-leave.#{$PF}-leave-active {
  animation-name: ETFadeLeave;
}

$PZ: $P + '-zoom';

@include ETAnimationMixin($PZ);

/**
 * animation part
 * ETFadeEnter
 * ETFadeLeave
 */
@keyframes ETFadeEnter {
  0% {
    transform: translateY(-10px);
    opacity: 0;
  }

  to {
    transform: translateY(0);
    opacity: 1;
  }

  // 0% {
  //   transform: scale(0.2);
  //   opacity: 0;
  // }

  // to {
  //   transform: scale(1);
  //   opacity: 1;
  // }
}

@keyframes ETFadeLeave {
  to {
    transform: translateY(-10px);
    opacity: 0;
  }

  // 0% {
  //   transform: scale(1);
  // }

  // to {
  //   transform: scale(0.2);
  //   opacity: 0;
  // }
}


实际使用，可参考 Message、modal 组件
const ETMessage = (config: any) => {
  // tmp prefix
  const prefix = 'et';

  const pf = `${prefix}-message`;
  const { content, duration = 2000, type = 'warn' } = config;

  let wrap = Q(`.${pf}-wrap`);

  if (!wrap) {
    wrap = CE('div');
    wrap.className = `${pf}-wrap`;
    document.body.appendChild(wrap);
  }

  const t = `${pf}-${type}`;

  const msg = htmlToElement(`
    <div class='${pf}'>
      <div class='${pf}-content ${t}'>
        ${content}
      </div>
    </div>
  `);

  wrap.appendChild(msg);

  ETFade({
    el: msg,
    isEnter: true,
  });

  let hasQuit = false;

  const handleClick = () => {
    if (hasQuit) {
      return;
    }

    hasQuit = true;

    ETFade({
      el: msg,
      callback: () => {
        wrap.removeChild(msg);
      },
    });
  };

  msg.addEventListener('click', handleClick);

  setTimeout(() => {
    handleClick();
  }, duration);
};


import * as React from 'react';
import * as ReactDOM from 'react-dom';

import { dom } from '@Utils';

const { addClass, removeClass, ETFade, ETZoom, setTransformOrigin, offset } = dom;

const { useEffect, useState, useRef } = React;

const confirm = (config: any) => {
  let div = document.createElement('div');

  if (config.id) {
    div.id = config.id;
  }

  if (config.targetParent) {
    config.targetParent.appendChild(div);
  } else {
    document.body.appendChild(div);
  }

  function close(...args: any) {
    destroy(...args);
  }

  function destroy(...args: any) {
    const unmountResult = ReactDOM.unmountComponentAtNode(div);

    if (unmountResult && div.parentNode) {
      div.parentNode.removeChild(div);
    }

    if (config.onCancel) {
      config.onCancel(...args);
    }
  }

  function render(props: any) {
    /**
     * https://github.com/ant-design/ant-design/issues/23623
     *
     * Sync render blocks React event. Let's make this async.
     */
    setTimeout(() => {
      ReactDOM.render(<Modal {...props} />, div);
    });
  }

  let currentConfig = { ...config, close, visible: true, wrap: div };

  render(currentConfig);
};

/**
 * title?: string           弹窗标题
 * content: any             弹窗主要内容
 * initCallback?: () => any 初始化函数
 * okText?: string          提交按钮文本
 * cancelText?: string      取消按钮文本
 * onOK?: () => any         提交后逻辑, 可以不传, 就当默认关闭
 * mp?: Object              鼠标点击位置 mousePosition
 */
const Modal = (props: any) => {
  const { title, content, initCallback, okText, cancelText, onOK, close, mp } = props;

  const [visible, setVisible] = useState(props.visible);

  const maskRef = useRef(null);
  const modalRef = useRef(null);

  const pf = 'et-modal';

  useEffect(() => {
    addClass('et-scroll-forbidden', document.body);

    // 若使用下面这种方式注册事件, 事件的响应顺序就乱了
    // 那时, content 中组件的事件定义必须通过类似 useEffect(() => { ... }, []) 的形式
    // 换句话说, 通用组件的编码形式会被限定, 会给开发工作带来额外负担
    // wrap &&
    //   wrap.addEventListener('click', () => {
    //     console.log('enter wrap clik');
    //     // setVisible(false);
    //   });
    // modalRef.current &&
    //   modalRef.current.addEventListener(
    //     'click',
    //     (e) => {
    //       // e.stopPropagation();
    //       console.log('enter stopPropagation');
    //     },
    //     false
    //   );

    const modal = modalRef.current;
    if (mp) {
      const elOffset = offset(modal);
      setTransformOrigin(modal, mp.x - elOffset.left + 'px ' + (mp.y - elOffset.top) + 'px');
    } else {
      setTransformOrigin(modal, '');
    }

    if (initCallback) {
      initCallback();
    }

    const handleEscQuit = (e: any) => {
      if (e.keyCode === 27) {
        handleClose();
      }
    };

    document.body.addEventListener('keydown', handleEscQuit);

    return () => {
      document.body.removeEventListener('keydown', handleEscQuit);
    };
  }, []);

  useEffect(() => {
    let method = mp ? ETZoom : ETFade;

    if (visible) {
      if (maskRef.current && modalRef.current) {
        ETFade({
          el: maskRef.current,
          isEnter: true,
        });

        // removeClass('is-hidden', modalRef.current);

        method({
          el: modalRef.current,
          isEnter: true,
        });
      }
    } else {
      ETFade({
        el: maskRef.current,
      });

      method({
        el: modalRef.current,
        callback: () => {
          removeClass('et-scroll-forbidden', document.body);
          close();
        },
      });
    }
  }, [visible]);

  const handleClose = () => {
    setVisible(false);
  };

  const handleOK = () => {
    if (onOK) {
      onOK();
    }

    handleClose();
  };

  const stopPropagation = (e: any) => {
    e.stopPropagation();
  };

  return (
    <>
      <div className={`${pf}-mask`} ref={maskRef} onClick={handleClose}></div>
      <div className={`${pf}-wrap`}>
        <div className={`${pf}`} ref={modalRef} onClick={stopPropagation}>
          <div className={`${pf}-content`}>
            <div className={`${pf}-close ${pf}-btn-close`}></div>

            {title && (
              <div className={`${pf}-header`}>
                <div className={`${pf}-title`}>{title}</div>
              </div>
            )}

            <div className={`${pf}-body`}>{content}</div>

            <div className={`${pf}-footer`}>
              {cancelText && (
                <div className={`et-btn is-bounce ${pf}-btn ${pf}-btn-cancel`} onClick={handleClose}>
                  {cancelText}
                </div>
              )}
              {okText && (
                <div className={`et-btn is-bounce ${pf}-btn ${pf}-btn-submit`} onClick={handleOK}>
                  {okText}
                </div>
              )}
            </div>
          </div>
        </div>
      </div>
    </>
  );
};

Modal.confirm = confirm;

export default Modal;


例子在这里了，若有时间，最好自己动手试一试
