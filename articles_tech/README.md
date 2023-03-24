# Technoligical Things 技术相关的东西

记录、总结一些技术相关内容


* 救助情报站快速搭建


带弹幕播放器


## Index 目录

* 0001.md -> Code Editors 四大编辑器攻略
* 0002.md -> Clojure & ClojureScript 学习笔记
* 0003.md -> Shell 命令
* 0004.md -> Sass、Less 学习笔记
* 0005.md -> SQL 手册
* 0006.md -> Git 手册
* 0007.md -> Three.js 学习笔记
* 0008.md -> JS 不成文笔记
* 0009.md -> Web 不成文笔记
* 0010.md -> sed & awk
* 0011.md -> Typescript React HMR 要点
* 0012.md -> 概念
* 0013.md -> React 笔记
* 0014.md -> TypeScript 笔记
* 0015.md -> 项目脚手架折腾回忆录
* 0016.md -> umi 备忘
* 0017.md -> Pinterest 插件分析
* 0018.md -> Chrome Extension/Plugins 插件开发笔记
* 0019.md -> Prettier 折腾小记
* 0020.md -> HTTP 学习笔记
* 0021.md -> Koa 学习笔记
* 0022.md -> Flutter 学习笔记
* 0023.md -> Webpack 笔记
* 0024.md -> Electron 笔记
* 0025.md -> Polyfill 合集
* 0026.md -> ECMAScript 笔记
* 0027.md -> 工具库笔记
* 0028.md -> PurgeCSS 笔记
* 0029.md -> Regex 正则笔记
* 0030.md -> Shell 编程学习笔记
* 0031.md -> Web 过渡动画笔记
* 0032.md -> 网络及代理学习笔记
* 0033.md -> ffmpeg 学习笔记
* 0034.md -> AI 学习笔记
* 0035.md -> 图形图像处理相关学习笔记
* 0036.md -> Python 学习笔记
* 0037.md -> Node 学习笔记
* 0038.md -> Nginx 学习笔记
* 0039.md -> 原神笔记
* 0040.md -> Taichi 学习笔记
* 0041.md -> 音视频编解码学习笔记
* 0042.md -> handlebars 学习笔记
* 0043.md -> ssh 笔记
* 0044.md -> Unity 学习笔记
* 0045.md -> Blender 学习笔记
* 0052.md -> VSCode 插件开发笔记
* 0053.md -> Docker 学习笔记
* 0054.md -> Nextjs 学习笔记
* 0055.md -> Apache 学习笔记
* 0095.md -> Wifi
* 0096.md -> 移动端代理、调试相关备忘
* 0097.md -> CSS 关键备忘
* 0098.md -> PC 主机 DIY 笔记
* 0099.md -> Windows 环境配置
* 0100.md -> AutoHotKey AHK & AppleScript 笔记
* 0101.md -> 云服务器环境配置
* 0110.md -> 常用软件安装及设置
* 5000.md -> 典型代码笔记
* 6000.md -> 新手引导
* 9999.md -> Chrome Snippets 目录




```js
// 获取所有标签页 tabs
const getTabs = () => {
  return new Promise((resolve) => {
    chrome.tabs.query({}, (tabs) => {
      resolve(tabs);
    });
  });
};

// 根据 id 关闭指定 tab
closeTab = (id) => {
  chrome.tabs.remove(id, function () {
    console.log('should be successful');
  });
};
```




【都市难民】
【无缘社会是什么】
【人与社缘】
【人与地缘】
【人与血缘】
【无缘社会下的现象】
【无缘社会与独身经济】
【无缘社会下的思考】
【无缘社会与新缘结】

<script type="text/javascript" src="/manifest.js"></script>
<script type="text/javascript" src="/vendor.js"></script>

    name: 'vendor',
    minChunks: function (module) {
      return (
          module.resource &&
          /\.js$/.test(module.resource) &&
          module.resource.indexOf(
            path.join(__dirname, './node_modules')
          ) === 0
      );
    }
  }),
  new webpack.optimize.CommonsChunkPlugin({
    name: 'manifest',
    chunks: ['vendor', 'main']
  }),

  https://juejin.cn/post/6986453616517185567