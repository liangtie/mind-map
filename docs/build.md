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

```bash
cd web
npm install
npm run build
# 这一步会报错This dependency was not found:
#* quill-delta in ../simple-mind-map/src/plugins/RichText.js

```

## 运行

### simple-mind-map

```bash
npm run wsServe

```

### web

## 调试
