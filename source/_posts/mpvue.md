---
title: 微信小程序搭建 mpvue
date: 2019-04-18 10:26:53
categories: 开发
summary: 用 vue 写小程序，使用 mpvue 框架重写 WeUI。
tags:
    - 前端
---

# mpvue
Vue.js in mini program
项目地址 [mpvue](https://github.com/Meituan-Dianping/mpvue)
> 用 vue 写小程序，使用 mpvue 框架重写 WeUI。
mpvue 是由美团点评开源的，一个使用 Vue.js 开发小程序的前端框架，目前支持 微信小程序、百度智能小程序，头条小程序 和 支付宝小程序。 框架基于 Vue.js，修改了的运行时框架 runtime 和代码编译器 compiler 实现，使其可运行在小程序环境中，从而为小程序开发引入了 Vue.js 开发体验。

## 主要特性
使用 `mpvue` 开发小程序，你将在小程序技术体系的基础上获取到这样一些能力：

- 彻底的组件化开发能力：提高代码复用性
- 完整的 `Vue.js` 开发体验
- 方便的 `Vuex` 数据管理方案：方便构建复杂应 用
- 快捷的 `webpack` 构建机制：自定义构建策略、开发阶段 hotReload
- 支持使用 npm 外部依赖
- 使用 `Vue.js` 命令行工具 vue-cli 快速初始化项目
- H5 代码转换编译成小程序目标代码的能力


# 项目初始化
注：如果没有安装node环境的请先去网上下载node.js下来安装，安装后默认安装npm了
- 到你要建项目的目录下打开cmd窗口（快捷方法：打开到目录后按住键盘shift，然后点击鼠标右键选择在此处打开powershell窗口即可）

- npm默认从外网下载包，可能会比较慢，可以换成国内的下载地址，如下

> npm set registry https://registry.npm.taobao.org/
这样就换成国内的淘宝镜像下载了

> npm install -g vue-cli
全局安装vue-cli，vue的官方脚手架

> npm install -g webpack
安装webpack打包管理

> npm install -g vue
全局安装vue框架

- 安装完上面的必须组件后，我们就进去正题了，初始化mpvue框架
> vue init mpvue/mpvue-quickstart my-project