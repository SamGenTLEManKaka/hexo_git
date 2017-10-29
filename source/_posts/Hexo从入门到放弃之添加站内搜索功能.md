---
title: Hexo从入门到放弃之添加站内搜索功能
date: 2017-07-16 17:48:10
tags: 
	- Hexo
	- Local Search
	- Node.js
updated:
comments: true
categories: 
	- Hexo
---
> 博客内文章太多了，一个一个找很费时间，需要一个搜索功能来快速查找站内关键词，我使用的是Local Search

<!--more-->
# Local Search
1、安装 hexo-generator-search
在根目录下执行命令：
```cmd
$ npm install hexo-generator-search --save
```
2、安装 hexo-generator-searchdb
在根目录下执行命令：
```cmd
$ npm install hexo-generator-searchdb --save
```
#配置生效
1、打开根目录下的配置文件_config.yml，添加以下配置内容：
```cmd
search:
  path: search.xml
  field: post
  format: html
  limit: 10000
```
2、打开主题配置文件_config.yml，修改local_search配置项为true：
```cmd
local_search:
  enable: true
```
然后重新发布hexo即可在导航栏看到“搜索”按钮，点击就可以搜索了。