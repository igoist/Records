## Log of my daily works 谈工作，谈学习




### 2017.07.17
<p>今天 webpack HMR 原型终于配出来了（老子终于也有资格说 XXXX 是个好东西了）</p>
<p>这里留点备注，既可以方便自己回顾，也可以替有缘人指点一下迷津（也许可去做一个从零开始学 webpack 的系列小教程）</p>
<p>学 webpack，有很重要的几点需要首先理解清楚</p>
<p>在部署项目的时候，一般在服务器上让部署者直接执行 webpack（或 gulp build, npm run build），生成我们的目标 bundle</p>
<p>但是在本地进行开发的时候，不可能改了一两行代码就执行一次编译与生成 bundle，尤其对于具备一定规模的正式项目，不用多解释</p>
<p>于是，开发环境（也就是能够在修改一两行代码后很自动化、快速地对应到目标文件，甚至做到 HMR）的合理部署显得非常重要</p>
<p>主要还是得安利 webpack-dev-server</p>

<p>这里不讲最最基本的几个<code>loader</code>，也不讲 webpack 能够通过<code>entry</code>指定去打包文件</p>
<p>先不提 react-hot-loader</p>

<p>（之前主要也是不理解，踩坑踩得要死要活）</p>
<p>在大概是看到官方文档前，一直并不晓得 webpack-dev-server 运行时内容不会真的编译到 dist</p>
<p>这同样意味着，运行时，它也不会读取 dist 下内容（可通过<code>contentBase</code>指定目标 dir）</p>
<p>因为为了达到快速编译的目的，它原理是将编译的内容都暂存在内存当中</p>

<p>webpack-dev-server 搞清楚，配清楚了，react-hot-loader 只不过就是加个依赖、加个 loader 的事情</p>
...
<p>这么长就以来一直纠结来纠结去，现在也应该是想得比较清楚了</p>
<p>如今做前端开发，自己本地玩的一些项目，可以采用 tab 缩进 spaces: 2、统一带冒号、都用 es6 的方式来进行开发</p>
<p>而公司项目，spaces: 4，也同意带冒号，都用 es6</p>
<p>咦吁兮！似不似区别不大呀？！</p>


### 2017.07.12
<p>Shit!</p>
<p>I hate bootstrap file-input!</p>


### 2017.07.08
<p>（明明当初是考虑到技术与生活分开记的）</p>
<p>这几个月期间，看过不少讲 gulp、webpack 的文章</p>
<p>说实话，直到今天，以多页面项目来讲，我尚且只能简单地使用 gulp 去罗列各个需要的文件、目录</p>
<p>对于 SPA，或者用 browserify，或者 webpack，都有现成实现方案</p>
<p>然而想在 React 项目中 hot reload，至今说不准问题所在</p>
<p>MPA 项目一旦需要逐步更新迭代，旧有的 gulp 打包方式完全不可行，于是才迫切需要早点精通 webpack</p>
<p>我之前一直想问：设想一下，换成你，你会如何地指引过去刚开始接触打包、构建的自己，循序渐进地来学习这块内容？</p>
<p>......</p>


### 2017.06.05
<p>我能承认说我刚刚才学会用某工具单步调试？</p>


### 2017.06.02
<p>总算大致搞清楚 React 中 Redux 大致运作以及使用方式。</p>
<p>工作什么的随它去吧，开始自己的项目重构。</p>


### 2017.06.01
<p>前些天吃了简历无脑乱写的亏。</p>
<p>不得已，有点紧迫，这些天只能代码少写些，必得等搞定这档子破事情，定下工作，再专心来写代码。</p>


### 2017.05.31
<p>现阶段最主要的，便是学会配合 Redux、React Router 这些来构建自己的 SPA</p>


### 2017.05.29
<p>[之前想实现的字幕效果基础部分](http://localhost/~egoist/Web/Demo%20of%20web/Font/Practice/t003.html)，也是换成位移的方式来模拟，</p>
<p>对<code>.wrap</code>需要设置<code>overflow: hidden</code>，而覆盖条颜色需要跟背景色保持一致。另外要是想实现最初所想的字幕效果，这边的位移得塞到<code>kf-animition</code>当中去，根据字数拆分<code>steps(x)</code>，并且对单个的字做处理</p>


### 2017.05.28
<p>这天还是回顾了一下前面没看完的文章，打好了那个结合 Redux 跟 ImmutableJS 的 todo 例子的架子，准备完成后续内容</p>
<p>知乎上看到那个问题，想法跟我之前差不多，重新想了想，发现可以用位移的方式来模拟</p>


### 2017.05.27
<p>最后还是根据这篇 [搭建 React , Babel 和 Webpack](http://fuxiaohei.me/2016/5/5/react-babel-webpack-start.html)，加入了 'babel-preset-es2015' 跟 'babel-preset-react' 才通过编译</p>
<p>然而这一篇更加深入 [webpack 2 打包实战](https://zhuanlan.zhihu.com/p/27046322)</p>


### 2017.05.26
<p>Learn about yarn from this [article](https://code.facebook.com/posts/1840075619545360)</p>
<p>and those types, [dependency-types](https://yarnpkg.com/lang/en/docs/dependency-types/)</p>


### 2017.05.25
<p>现在的人基本都知道所谓工程化</p>
<p>感觉项目构建这块实在很重要</p>
<p>一边深入学习 react，辅以 Flux（Redux）</p>
<p>也通过相关项目，开始重新系统学习 npm，yarn，gulp，webpack</p>


### 2017.05.23
> None for yet, because I was rushing for resume.




### 在此列举一些社区
* [cnode](http://cnodejs.org/)
* [开源中国 React](https://www.oschina.net/question/tag/react) 用了 git 账号
