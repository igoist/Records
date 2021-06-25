# 气泡卡片 Popover

## JS

可参考 live common.js 中的 bindPopoverEvent

```js
let bindPopoverEvent = (config) => {
  let target = config.target;
  let parent = config.parent;

  function handleLeave() {
    target.classList.remove('zoom-big-leave-active');
    target.classList.remove('zoom-big-leave');
    target.classList.add('popover-hidden');

    target.removeEventListener('animationend', handleLeave);
    document.body.removeEventListener('click', handleBlur);
  }

  function handleBlur() {
    target.classList.add('zoom-big-leave');
    target.classList.add('zoom-big-leave-active');
    target.addEventListener('animationend', handleLeave);
  }

  function handleEnter() {
    target.classList.remove('zoom-big-enter');
    target.classList.remove('zoom-big-enter-active');
    target.removeEventListener('animationend', handleEnter);

    document.body.addEventListener('click', handleBlur, false);
  }

  function handle(e) {
    if (target.classList.contains('popover-hidden')) {
      target.addEventListener('animationend', handleEnter);
      target.classList.add('zoom-big-enter');
      target.classList.add('zoom-big-enter-active');
      target.classList.remove('popover-hidden');
    }

    if (!target.style.left) {
      target.style.left = $(parent).offset().left - target.offsetWidth + 38 + 'px';
      target.style.transformOrigin = target.offsetWidth + 'px -4px 0px';
    }

    // 该 if 语句及后面事件绑定为导入 popover 临时代码
    if (e.target === document.querySelector('.popover-item button')) {
      parent.removeEventListener('click', handle, false);
    }
  }

  parent.addEventListener('click', handle, false);
};
```