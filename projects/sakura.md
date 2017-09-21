# Sakura 项目备忘
<p>基本就是得配置好 Emacs，其余编辑器暂时没有看到好的方案</p>


## 项目启动
<p>关于 Emacs 配置参考...</p>
<p>第一步：打开文件，进入项目后，通过 cider-jack-in(, + ') 开启第一个 cider-repl</p>
<p>第二步：repl 中先后执行 (run)/(go)、(browser-repl)/(cljs-repl)，等待连接完成（后者需在 browser 中打开... 才能完成连接）</p>
<p>第三步：也就是最后，继续 cider-jack-in(, + ')，为执行 clj 文件新建第二个 repl 进程</p>


## UI 组件页热加载启动
<p>完成项目启动后，在 REPL 中输入如下</p>
```clojure
(start-autobuild "devcards")
```
服务启动后访问[该地址](http://localhost:3000/devcards.html)
