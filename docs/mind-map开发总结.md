# mind-map

## 介绍

mind-map 由两个项目组成：

1. simple-mind-map : 一个 js 思维导图库，不依赖任何框架，可以使用它来快速完成 Web 思维导图产品的开发。

开发文档：[https://wanglin2.github.io/mind-map/#/doc/zh/](https://wanglin2.github.io/mind-map/#/doc/zh/)。

2. web : 一个 Web 思维导图，基于思维导图库、Vue2.x、ElementUI 开发，可以操作电脑本地文件，可以当做一个在线版思维导图应用使用，也可以自部署和二次开发。

在线地址：[https://wanglin2.github.io/mind-map/](https://wanglin2.github.io/mind-map/)

## 环境

1. nodejs

https://nodejs.org/en/download/current

2. git

https://git-scm.com/downloads

3. vscode

https://code.visualstudio.com/download

## 拉取代码

```bash
git clone  https://github.com/wanglin2/mind-map.git

```

## 构建

### simple-mind-map

```bash

cd simple-mind-map
npm install

```

### web

构建 web 前需要修改 web/package.json，在 dependencies 中添加 "simple-mind-map": "file:../simple-mind-map" ，添加后的 dependencies 如下：

```json
  "dependencies": {
    "@toast-ui/editor": "^3.1.5",
    "codemirror": "^5.65.16",
    "core-js": "^3.6.5",
    "element-ui": "^2.15.1",
    "highlight.js": "^10.7.3",
    "katex": "^0.16.9",
    "v-viewer": "^1.6.4",
    "vue": "^2.6.11",
    "vue-i18n": "^8.27.2",
    "vue-router": "^3.5.1",
    "vuex": "^3.6.2",
    "xlsx": "^0.18.5",
    "simple-mind-map": "file:../simple-mind-map"
  },
```

```bash
cd web
npm install
npm run build

```

## 运行

### simple-mind-map

```bash
npm run wsServe

```

### web

```bash

npm run serve

```

会在控制台输出类似如下内容：

App running at:

- Local: http://localhost:8080
- Network: http://192.168.50.107:8080

Note that the development build is not optimized.
To create a production build, run npm run build.

打开 http://localhost:8080 就可以访问了。
