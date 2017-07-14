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

然后就会在此目录下生成以下目录结构：
    
    ├── gulpfile.js               # gulp任务配置
    ├── package.json              # 项目配置
    ├── README.md                 # 项目说明
    ├── src                       # 源码目录
    │   ├── css/                  # css资源
    │   ├── html/                 # 入口文件html
    │   │   ├── pageA.html          # 入口文件a
    │   │   ├── pageB.html          # 入口文件b
    │   │   ├── pageC.html          # 入口文件c
    │   ├── img/                  # 图片资源
    │   ├── include/              # 公共引用html(公共头部，尾部等)
    │   ├── js                    # js&jsx资源
    │   │   ├── entry/            # 页面入口js
    │   │   │   ├── pageA.js            # a页面入口
    │   │   │   ├── pageB.js            # b页面入口
    │   │   │   ├── pageC.js            # c页面入口
    │   │   ├── helpers/          # 业务相关的辅助模块,例如函数
    │   │   ├── lib/              # 没有存放在npm的第三方库或者下载存放到本地的基础库，如jQuery、Zepto、Vue等
    │   │   └── utils/            # 业务无关的辅助工具
    │   ├── scss/                 # scss资源
    │   ├── pathmap.json          # 手动配置某些模块的路径，可以加快webpack的编译速度
    ├── webpack.config.allinone.js    # webpack配置
    ├── webpack.config.js         # 正式环境webpack配置入口
    └── webpack-dev.config.js     # 开发环境webpack配置入口


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
