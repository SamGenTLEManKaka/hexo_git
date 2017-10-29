---
title: Hexo从入门到放弃之添加顶部加载条
date: 2017-07-28 08:26:34
tags: 
	- bootcss
	- Hexo
	- Node.js
updated:
comments: true
categories: 
	- Hexo
---
> 博客内容太多，加载太慢，需要一个进度条来显示加载进度，提高用户体验。

<!--more-->

# 具体实现方法

打开主题配置文件下的 layout/_partials/head.swig文件，以下代码
```cmd
<script src="//cdn.bootcss.com/pace/1.0.2/pace.min.js"></script>
<link href="//cdn.bootcss.com/pace/1.0.2/themes/pink/pace-theme-flash.css" rel="stylesheet">
```
就已经设置好了默认的进度条
# 进阶
更改进度条颜色
```cmd
<style>
    .pace .pace-progress {
        background: #1E92FB; /*进度条颜色*/
        height: 3px;
    }
    .pace .pace-progress-inner {
         box-shadow: 0 0 10px #1E92FB, 0 0 5px     #1E92FB; /*阴影颜色*/
    }
    .pace .pace-activity {
        border-top-color: #1E92FB;    /*上边框颜色*/
        border-left-color: #1E92FB;    /*左边框颜色*/
    }
</style>
```
这里可以自定义进度条的一些颜色属性