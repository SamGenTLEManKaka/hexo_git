---
title: (四)Hexo从入门到放弃之更换Next主题
date: 2017-07-15 15:53:50
tags: 
	- Hexo
	- github
	- Next
	- Node.js
updated:
comments: true
categories: 
	- Hexo
---
> 独一无二是个性，打LOL宁愿花钱买皮肤都不愿意用经典皮肤，Hexo有很多种免费皮肤可以随意更换，这里我选择Next主题

<!--more-->
# Next主题
1、下载
    点击[**Next代码仓库**](https://github.com/iissnan/hexo-theme-next/releases)选择版本下载Next主题源代码，版本当然选择最新的稳定版
2、安装
	下载下来的压缩包解压后放至Hexo根目录的themes\目录下
	打开Hexo根目录名为_config.yml的全局配置文件，找到theme:这个配置项，把主题目录名称粘贴上去
```cmd
theme: hexo-theme-next-5.0.1
```
3、重新上传下Hexo可以查看效果
```cmd
hexo g
hexo d
```
4、进阶
   更多个性化设置访问[**Next官网**](http://theme-next.iissnan.com/)