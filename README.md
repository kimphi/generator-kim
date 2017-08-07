# generator-kim
基于gulp+webpack的多页面前端项目生成器
------------

开始安装

首先确保自己已经安装了nodejs

然后安装yeoman

```js
npm install -g yo
```
然后安装脚手架

```js
npm install -g generator-kim
```

在自己的空项目中运行：

```js
yo kim
```

使用这个脚手架的好处

```js
1、模块化开发（一切皆模块，包括css,js,image）

2、模块复用，易迁移

3、区分开发模式和生成模式

4、开发模式下能同步刷新（提高开发效率）

5、开发模式下能配置代理转发（解决本地开发跨域问题））

6、生产模式下自动打包和压缩html,js,css

7、自动根据文件内容生成md5戳（解决缓存）

8、js语法校验
```
