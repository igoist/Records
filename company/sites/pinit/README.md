# 主站 Pinit 笔记


##....

* .dot 模板
* a.x 禁用 target blank
* is_private... 1=? 2=? 3=? 这类数据库中字段直接找对应 Modal，如 lib/models/board/board.js，内有注释


点 广告管理-广告推广管理 跳转有问题

叉有问题

## 内容索引

* 0000.md -- Google、百度、第四范式广告等广告相关备忘
* 0001.md -- 采集插件相关
* 0002.md -- 统计监测相关
* 0003.md -- 英尼 Ins 备忘
* 0004.md -- 详情页相关
* 0005.md -- 路由相关
* 0006.md -- Mootools 笔记
* 0007.md -- Waterfall 初始化、运行机制 & 采集详情页重构笔记
* 0008.md -- 全站广告系统重构笔记
* 0009.md -- 新手功能引导重构笔记
* 000x.md -- views/base/people_profile.pug

## 备忘

base/selector - Selector 选择器

lvs nginx 负载均衡

Freddie Mercury 1985 年 Live Aid 演唱会版本

https://www.zhihu.com/search?type=content&q=unrar  unrar

http://pinban.com/boards/27451236/?kkfa8bf6&limit=20&wfl=1

http://pinban.com/home/?kkfa8bf8&limit=20&wfl=1

* 错误收集


## 关于新整理的组件

最初尝试了将包括 js script 逻辑的大部分内容都写对应的 hb-xx 模版中

然后发现当尝试通过如下方式注入内容时

```js
Elements.from(modalStr).inject(div);

// ...
Elements.from(config.modalInner).inject(modalBody);

// 或
div.innerHTML = modalStr;

modalBody.innerHTML = config.modalInner;
```

要么 script 部分会被无视(直接从字符串中过滤？)

要么估计是 chrome 的安全策略相关, 闭包没有被执行


所以思来想去, 最后决定每个组件的模板只做模板该做的事, 而逻辑部分, 应当单独在 common.js 中定义一个处理初始化、事件绑定相关内容的函数

实现过程中区别的点, 模板、逻辑分离后, 为了定位元素, 组件 id 以及其他可能的参数会需要在引用模板处及执行逻辑函数处各传一次

## docker ?

删除 redis 缓存

```
huaban redis start

keys *

keys rate*(寻找匹配项)

del rate:limit:post:2462300354:172.17.0.1 rate:limit:post:3166869443:172.17.0.1
```