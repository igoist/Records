# 通知框 Notification


## JS

*XXX*

```js
/**
 * wrapPosition?: string 如 topRight
 * title: string         通知框标题
 * desc: string          通知框内容
 * onClick?: any         点击(查看)通知回调
 * onClose?: any         点击关闭回调
 * duration?: number     若干毫秒后自动关闭
 */
var initNotification = function (config) {
  var wrapPosition = config.wrapPosition || 'topRight';

  var htmlStr = app.renderSync('base/hb-notification', {
    title: config.title,
    desc: config.desc,
  });

  var wrap = document.getElement('.hb-notification-wrap-' + wrapPosition);

  if (!wrap) {
    wrap = document.createElement('div');
    wrap.className = 'hb-notification-wrap hb-notification-wrap-' + wrapPosition;
    document.body.appendChild(wrap);
  }

  Elements.from(htmlStr).inject(wrap);

  var notification = wrap.getElement('.hb-notification');
  var btnNotification = notification;
  var btnClose = wrap.getElement('.hb-notification-close');

  var handleFadeIn = function () {
    notification.addClass('hb-notification-fade-appear');
    notification.addClass('hb-notification-fade-appear-active');

    var handleFadeInEnd = function () {
      notification.removeClass('hb-notification-fade-appear-active');
      notification.removeClass('hb-notification-fade-appear');
      notification.removeEventListener('animationend', handleFadeInEnd);
    };

    notification.addEventListener('animationend', handleFadeInEnd);
  };

  handleFadeIn();

  var handleFadeout = function (callback) {
    notification.addClass('hb-notification-fade-leave');
    notification.addClass('hb-notification-fade-leave-active');

    var handleFadeInEnd = function () {
      notification.removeClass('hb-notification-fade-leave-active');
      notification.removeClass('hb-notification-fade-leave');
      notification.removeEventListener('animationend', handleFadeInEnd);

      if (callback) {
        callback();
      }
    };

    notification.addEventListener('animationend', handleFadeInEnd);
  };

  var handleClick = function () {
    handleFadeout(function () {
      notification.dispose();

      if (config.onClick) {
        config.onClick();
      }
    });
  };

  var handleClose = function (e) {
    e.stop();

    handleFadeout(function () {
      notification.dispose();

      if (config.onClose) {
        config.onClose();
      }
    });
  };

  btnNotification && btnNotification.addEvent('click', handleClick);
  btnClose && btnClose.addEvent('click', handleClose);

  if (config.duration) {
    setTimeout(function () {
      btnClose && btnClose.click();
    }, config.duration);
  }
};
```

## CSS

```css
/* Notification start */
.hb-notification-wrap,
.hb-notification *,
.hb-notification {
  margin: 0;
  box-sizing: border-box;
  padding: 0;
}

.hb-notification-wrap {
  position: fixed;
  margin-right: 24px;
  line-height: 1.5715;
  list-style: none;
  color: rgba(0,0,0,.85);
  font-size: 14px;
  font-variant: tabular-nums;
  -webkit-font-feature-settings: "tnum";
  font-feature-settings: "tnum";
  z-index: 90;
}

.hb-notification-wrap.hb-notification-wrap-topRight {
  top: 48px;
  right: 0;
  bottom: auto;
}

.hb-notification {
  cursor: pointer;
  position: relative;
  margin-bottom: 16px;
  margin-left: auto;
  border-radius: 8px;
  padding: 18px 20px;
  max-width: 312px;
  background: #fff;
  box-shadow: 0 3px 6px -4px rgb(0 0 0 / 12%), 0 6px 16px 0 rgb(0 0 0 / 8%), 0 9px 28px 8px rgb(0 0 0 / 5%);
  overflow: hidden;
  transition: all 0.24s ease-in-out;
}

.hb-notification-fade-out {
  opacity: 0;
  transform: translateY(-10%);
}

.hb-notification-content {
  font-family: -apple-system, 'Helvetica Neue', Tahoma, sans-serif;
}

.hb-notification-title {
  margin-bottom: 10px;
  padding-right: 8px;
  max-height: 40px;
  line-height: 20px;
  font-size: 16px;
  font-weight: bold;
}

.hb-notification-desc {
  max-height: 54px;
  line-height: 18px;
  color: #7b7b7b;
  font-size: 14px;
  text-align: left;
  overflow: hidden;
}

.hb-notification-close {
  position: absolute;
  top: 8px;
  right: 8px;
  width: 16px;
  height: 16px;
  background-image: url(/img/icons/ic-hb-notification-close.svg);
  background-position: center 0;
  background-repeat: no-repeat;
  background-size: 16px 16px;
}

.hb-notification-fade-appear,
.hb-notification-fade-enter {
  opacity: 0;
  animation-play-state: paused;
}

.hb-notification-fade-appear,
.hb-notification-fade-enter,
.hb-notification-fade-leave {
  animation-duration: 0.24s;
  animation-timing-function: cubic-bezier(0.645, 0.045, 0.355, 1);
  animation-fill-mode: both;
}

.hb-notification-fade-leave {
  animation-duration: 0.2s;
  animation-play-state: paused;
}

.hb-notification-fade-appear.hb-notification-fade-appear-active,
.hb-notification-fade-enter.hb-notification-fade-enter-active {
  animation-name: HBNotificationFadeIn;
  animation-play-state: running;
}

.hb-notification-fade-leave.hb-notification-fade-leave-active {
  animation-name: HBNotificationFadeOut;
  animation-play-state: running;
}

@keyframes HBNotificationFadeIn {
  0% {
    left: 110%;
    opacity: 0;
  }

  to {
    left: 0;
    opacity: 1;
  }
}

@keyframes HBNotificationFadeOut {
  0% {
    max-height: 150px;
    margin-bottom: 16px;
    opacity: 1;
  }

  to {
    max-height: 0;
    margin-bottom: 0;
    padding-top: 0;
    padding-bottom: 0;
    opacity: 0;
  }
}
/* Notification end */
```