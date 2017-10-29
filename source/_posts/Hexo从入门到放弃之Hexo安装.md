---
title: (一)Hexo从入门到放弃之Hexo安装
date: 2017-02-04 21:24:33
tags: 
	- Hexo
	- github
	- Node.js
updated:
comments: true
categories: 
	- Hexo
---
> Hexo是部署简单的静态博客，可以配合github page的免费空间，多种主题搭配选择，使用Markdown语法，稍微有点计算机基础都可以搭建。

<!--more-->
***
# 配置环境
1、Node.js
去[**Node官网**](https://nodejs.org/en/)下载最新版本，安装一路狂点下一步就安装好了。
2、git
去[**git下载页**](https://git-scm.com/downloads)下载git，安装。
# hexo安装
安装好Node.js和git后，找一个目录（准备存放Hexo的目录），点击鼠标右键，选择“**Git Bash Here**”，输入以下命令安装Hexo
```cmd
npm install hexo-cli -g
```
小等一会后继续输入以下命令
```cmd
hexo init
```
Hexo所有的文件都被创建在了当前目录下，继续输入安装相关依赖：
```cmd
npm install
```
到现在Hexo全部组件都安装完成了，现在可以尝试开启服务
```cmd
hexo server
```
如果看到下面的提示，说明服务开启成功了
```cmd
INFO  Start processing
INFO  Hexo is running at http://localhost:4000/. Press Ctrl+C to stop.
```
就可以打开浏览器，输入：localhost:4000，查看自己的Hexo博客网站了