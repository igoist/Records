# （本期的题目是：）Chrome Extension 入门

*大纲*

* 大致讲一下入口文件 manifest.json
* 几个权限的说明
* 实例
* 结尾


manifest.json 示例

```json
{
  "name": "IEXManager",
  "description": "It means igoist's extensions management tool.",
  "version": "1.0.0",
  // ? background 正常情况得用到，虽然也可以不填
  "background": {
    "scripts": ["js/background.bundle.min.js"],
    "persistent": false
  },
  "icons": {
    "32": "img/gear_large.svg",
    "48": "img/icon.png",
    "128": "img/icon-128.png"
  },
  // ?
  "content_scripts": [
    {
      // 可以使用 '<all_urls>' 替代
      "matches": ["*://*/*"],
      "run_at": "document_end",
      "js": ["dll/react.dll.js", "js/demo.bundle.min.js"],
      "css": ["css/IDemo.css"],
      "exclude_matches": ["http://127.0.0.1:3333/*", "https://*.yupoo-dev.cn/*"]
    }
  ],
  "manifest_version": 2,
  "content_security_policy": "script-src 'self' 'unsafe-eval'; object-src 'self';",
  "browser_action": {
    "default_icon": "img/gear_large.svg",
    // ? 很多都是直接用插件名，或者通过 js 注入 i18n
    "default_title": "自定义标签页管理工具,
    "default_popup": "popup.html"
  },
  // ? 多语言
  "default_locale": "zh_CN",
  "permissions": ["activeTab", "tabs", "storage", "sessions", "declarativeContent", "webNavigation", "*://*/*", "management"],
  // 这个需要特别说明一下
  "web_accessible_resources": ["css/pinit.min.css", "css/IAdB.css", "dll/reactForPinit.dll.js", "img/icon.png"]
}
```

background

content_scripts

content_security_policy 这部分就简单提一下吧

简称 CSP。顾名思义，这个规范与内容安全有关，主要是用来定义页面可以加载哪些资源，减少 XSS 的发生。

[content_security_policy ](https://developer.mozilla.org/en-US/docs/Mozilla/Add-ons/WebExtensions/Content_Security_Policy#default_content_security_policy)
[content_security_policy](https://developer.chrome.com/docs/apps/contentSecurityPolicy/)
[content_security_policy](https://developers.google.com/web/fundamentals/security/csp)
[content_security_policy](https://imququ.com/post/content-security-policy-reference.html)
[content_security_policy](http://www.ruanyifeng.com/blog/2016/09/csp.html)

default_locale

manifest_version(*这个不是特别重要，应该是去年 11 月左右更新至 3*)

[diff in v3](https://developer.chrome.com/docs/extensions/mv3/intro/)
[diff in v3](https://cezaraugusto.net/posts/what-changes-in-chrome-extension-manifest-v3/)
[diff in v3](https://stackoverflow.com/questions/63308160/how-to-migrate-manifest-version-2-to-v3-for-chrome-extension)

```json
// Manifest v2
"browser_action": {...}
"page_action": {...}

// Manifest v3
"action": {...}
```

```json
// Manifest v2
"background": {
 "scripts": ["js/background.js"]
}

// Manifest v3
"background": {
 "service_worker": "js/background.js"
}
```

```json
// Manifest v2
"content_security_policy": "script-src 'self' 'unsafe-eval'; object-src 'self'"

// Manifest v3
"content_security_policy": {
 "extension_pages": "script-src 'self' 'unsafe-eval'; object-src 'self'",
 "sandbox": "..."
}
```

[migrate to v3](https://blog.shahednasser.com/chrome-extension-tutorial-migrating-to-manifest-v3-from-v2/)


*web_accessible_resources*

举个例子，注入的 js、css（图片不确定也没有去验证，至少到目前暂时没有必要的理由） 在独立的插件线程（除非以 data base64 的形式，但并不算），渲染的结果一般在主线程，有些东西访问不到



```js
chrome.extension.getURL('/img/page.png');

{/* <img src="chrome-extension://effnflkmdihmiamnfmlfannoaolhgkab/img/page.png" /> */}
{/* <img src={chrome.extension.getURL('/img/page.png')} /> */}

// GET chrome-extension://invalid/ net::ERR_FAILED
```


多语言


## permissions

[权限列表](https://developer.chrome.com/docs/extensions/mv3/declare_permissions/)
[demo](https://github.com/GoogleChrome/chrome-extensions-samples/tree/main/mv2-archive/api)

这里首先要声明，很不好意思，准备的时间不大够，很多权限的解释我自己都还没看明白，

不过换句话说，相当于我写到现在，平常需要的权限主要也就那几个

很多对我来讲深不深入了解貌似没有特别的必要

主要还是遇到问题解决问题吧，这句话对不对，大家可以有自己的思考


'activeTab' or '<all_urls>'

* [chrome.downloads](https://developer.chrome.com/docs/extensions/reference/downloads/)
* [chrome.tabs](https://developer.chrome.com/docs/extensions/reference/tabs/)
* [chrome.management](https://developer.chrome.com/docs/extensions/reference/management/)
* storage - 访问 chrome.storage
* declarativeContent - 好像是说可以根据 url 是否匹配，来显示、隐藏插件 action/popup 按钮

```js
// tabs 演示用例
chrome.tabs.query({}, (tabs) => {
  console.log(tabs);
});

// management 演示用例
chrome.management.getAll((exs) => { console.log(exs); });

// history 演示用例
(() => {
  const microsecondsPerWeek = 1000 * 60 * 60 * 24 * 7;
  const oneWeekAgo = new Date().getTime() - microsecondsPerWeek;
  const callback = (historyItems) => {
    console.log('historyItems', historyItems);
  };

  chrome.history.search(
    {
      text: '', // Return every history item....
      startTime: oneWeekAgo, // that was accessed less than one week ago.
    },
    callback
  );
})();
```


## downloads

[downloads](https://github.com/GoogleChrome/chrome-extensions-samples/tree/main/mv2-archive/api/downloads)

* download_filename_controller
* download_links
* download_manager
* download_open
* downloads_overwrite


## tabs

move、交换标签页位置

pin 固定

回滚、记录历史、自定义日志、统计

```js
$.b.tabs.executeScript(o.tabId, {
  file: 'js/logic.js',
});
```


## management

这里做个脑筋急转弯小测试，考考大家，知道的先不要急着回答，为什么这里的 is-inset 不存在，有没有不知道的举个手


飞书知道的可以飞书里发我答案，


## 实例演示过程中的其他经验谈

*插件文件安装地址*

/Users/xxx/Library/Application Support/Google/Chrome/Default/Extensions

* 我自己历来大致的文件结构，

* 比方注入的内容可能会因为网站自己的一些机制，比如百度、google 搜索这种，dom 变动后被更新掉，怎么处理

* 关于通信（怎么来都可以，没有专门的限制，那么就要思考一些最佳实践... 比如谁谁谁怎么做的）

* 比较离谱的玩法，按键对应 fn，或者发事件到 server，然后 server 转 shell 执行

```js
function purify(nodes) {
  for (let node of nodes) {
    if (node.textContent.indexOf('热门内容, ') === 0) {
      node.querySelector('.TopstoryItem-rightButton').click();
      // node.parentNode.removeChild(node)
      console.log(node);
    }
  }
}

const mo = new MutationObserver((mutations) => {
  for (let mutation of mutations) {
    if (mutation.type === 'childList') {
      purify(mutation.addedNodes);
    }
  }
});

purify(QA('.TopstoryItem'));

if (Q('.TopstoryMain > div')) {
  mo.observe(Q('.TopstoryMain > div'), { childList: true });
}
```
## 结尾

*关于分层*


*links*

[jerryQu](https://imququ.com/post/series.html)
[otakustay](https://www.zhihu.com/people/otakustay/posts)
[...](http://febook.hzfe.org/awesome-interview/book2/browser-render-mechanism)
[...](https://colorhunt.co/)

[Simeon Vincent](https://www.youtube.com/watch?v=e_nEP--FOHE&ab_channel=JSConf)