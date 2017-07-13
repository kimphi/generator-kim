# webpack项目模板 #

## 安装依赖 ##

	$ npm install --registry=https://registry.npm.taobao.org

## 目录结构 ##

``` js
    .
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
```

## 开发要求 ##

约定/src/html/*.html为应用的入口文件，在/src/js/entry 目录下需有一个同名的js文件作为该文件的入口。


## 本地调试 ##

    $ npm run server

## 编译（测试环境） ##

    $ npm run build

## 编译（生产环境） ##

生产环境会对js混淆压缩，对css、html进行压缩，字符替换等处理

    $ npm run build-idc







