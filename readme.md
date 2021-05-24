Vue.js 2.5.17
ECMAScript 6
Node.js

Node Package Manager (npm)
- 查看安装版本
  - $ npm -v
- 初始化
  - $ npm init
- 使用默认值初始化
  - $ npm init -y
- 修改镜像地址
  - $ npm config set registry https://registry.npm.taobao.org
- 查看npm配置信息
  - $ npm config list
- 下载依赖
  - $ npm install jquery
- 下载依赖 特定版本
  - $ npm install jquery@2.1.x
- 全局安装
  - $ npm install --global webpack
  - $ npm install -g webpack
  - $ npm install -save-dev xxx

前端模块化开发, JavaScript之间的调用。
ES6的模块化无法在Node.js环境中执行，需要用Babel编辑成ES5后再执行。

Babel转码器
1. 安装
$ npm install -g babel-cli
$ babel --version
2. 配置文件.babelrc (module folder)
3. 安装es2015转换器
$ npm install -D babel-preset-es2015
4. 使用命令进行转码
$ babel src -d dist

Webpack打包工具
Webpack是一个前端资源加载/打包工具。它将根据模块的依赖进行静态分析， 然后将这些模块按照指定的规则生成对应的静态资源Webpack可以将多种静态资源js,css,less转换成一个静态文件，减少了页面的请求。
1. 安装
  - $ npm install -g webpack webpack-cli
  - $ webpack -v
3. 创建js文件 (webpack folder)
2. 创建配置文件webpack.config.js
3. 执行编译命令
  - $ webpack --mode=development

- 安装
  - $ npm install -D style-loader css-loader
- 创建css文件
  - e.g. see src/style.css and main.js


git clone https://github.com/PanJiaChen/vue-admin-template/tree/v3.8.0

$ npm install
$ npm run dev