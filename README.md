# Web屯

<p align="center">
  <img src="https://img.shields.io/badge/site-static-brightgreen" alt="static site" />
  <img src="https://img.shields.io/badge/built%20with-VuePress%201.9.10-blue" alt="VuePress" />
  <img src="https://img.shields.io/badge/content-frontend%20learning-orange" alt="frontend learning" />
  <img src="https://img.shields.io/badge/status-ongoing-success" alt="ongoing" />
</p>

一个面向前端基础学习的中文静态知识站点，围绕“系统学习，慢一点比较快”的思路，持续整理和沉淀前端基础内容。

## 目录

- [项目介绍](#项目介绍)
- [项目亮点](#项目亮点)
- [内容目录](#内容目录)
- [项目结构](#项目结构)
- [技术说明](#技术说明)
- [本地预览](#本地预览)
- [部署方式](#部署方式)
- [适合谁使用](#适合谁使用)
- [当前仓库说明](#当前仓库说明)
- [推荐补充内容](#推荐补充内容)
- [License](#license)

## 项目介绍

**Web屯** 是一个以前端基础知识为核心的学习型站点，内容覆盖 JavaScript、HTTP、Vue、数据结构以及部分框架与工程化主题。

这个项目的出发点很明确：相比只在遇到问题时零散搜索答案，更希望把常见知识点按主题系统整理下来，逐步形成可复习、可回顾、可持续补充的知识体系。

当前仓库保存的是站点的**构建产物**，也就是已经生成好的静态页面文件，因此可以直接部署到 **GitHub Pages** 或任意静态托管平台。

## 项目亮点

- 内容聚焦前端基础，主题清晰
- 以中文知识整理为主，适合日常复习与查阅
- 站点已构建完成，可直接部署
- 页面按专题划分，便于持续扩展
- 适合作为个人知识库、学习博客或静态文档站点参考

## 内容目录

目前站点主要包含以下内容方向：

### JS 基础

涵盖作用域、提升、闭包、`this`、数据类型、对象、原型链、继承、类型转换、`Promise`、`Event Loop` 等前端核心基础知识。

### HTTP 基础

包含 HTTP、HTTPS、缓存机制、常见请求头、跨域、TCP 与 UDP 等网络基础主题。

### Vue 基础

收录 Vue 中较常见的基础问题与原理型内容，例如双向绑定、`nextTick`、`v-if` 与 `v-for` 的使用问题等。

### 数据结构

用于补充前端学习过程中常见但又容易被忽略的数据结构基础认知。

### 框架相关

整理了一些更偏工程化和框架层面的内容，例如 Webpack 与 Vite 的区别、微前端方案、`qiankun` 等。

## 项目结构

```text
.
├── index.html                  # 站点首页
├── 404.html                    # 404 页面
├── README.md                   # 项目说明
├── assets/                     # 构建后的静态资源
│   ├── css/
│   ├── img/
│   └── js/
├── JS/                         # JavaScript 相关文章
├── HTTP/                       # HTTP 相关文章
├── Vue/                        # Vue 相关文章
├── DataStructure/              # 数据结构相关文章
└── 框架相关/                    # 框架与工程化相关文章
```

## 技术说明

从当前文件结构可以判断，这个项目是基于 **VuePress 1.9.10** 生成的静态站点。

项目特点如下：

- 静态输出，部署成本低
- 无需后端服务即可访问
- 适合托管在 GitHub Pages、Vercel、Netlify 或其他静态平台
- 适合做知识型博客、笔记站点和文档站点

## 本地预览

因为当前目录是已经构建好的静态文件，所以本地预览非常简单。

### 方式一：使用 Python

```bash
python3 -m http.server 8080
```

然后访问：

```text
http://localhost:8080
```

### 方式二：使用 Node.js

```bash
npx serve .
```

## 部署方式

### 部署到 GitHub Pages

如果这是你的 GitHub Pages 仓库，可以直接将当前静态文件推送到默认分支进行托管。

基本步骤如下：

1. 提交当前仓库内容
2. 推送到 GitHub 仓库
3. 进入仓库的 **Settings → Pages**
4. 选择发布分支
5. 保存设置并等待发布完成

如果仓库名是 `<username>.github.io`，通常会直接部署为用户主页站点。

### 部署到 Vercel

1. 将仓库导入 Vercel
2. Framework Preset 选择 **Other** 或保持默认
3. Output Directory 保持为空或使用当前根目录
4. 直接部署即可

### 部署到 Netlify / Cloudflare Pages

这类平台同样支持直接托管静态站点。

核心方式是：

- 连接仓库
- 构建命令留空，或不设置构建步骤
- 发布目录设置为项目根目录

### 部署到普通静态服务器

如果你使用的是 Nginx、Apache 或其他静态文件服务器，也可以直接把当前目录中的文件上传到网站根目录进行访问。

## 适合谁使用

这个项目适合以下场景：

- 想系统整理前端基础知识的个人开发者
- 想搭建个人前端学习站点或知识博客的人
- 需要一个静态知识站点参考结构的开发者
- 希望把碎片知识沉淀为长期资料库的学习者

