---
title: (三)Hexo从入门到放弃之发表文章
date: 2017-02-12 20:59:06
tags: 
	- Hexo
updated:
comments: true
categories: 
	- Hexo
---
> 博客最重要的就是发表文章了，Hexo的博客采用的是Markdown语法，只需要一个步骤就可以完成文章的发表。

<!--more-->
# 新建文章

进入到Hexo根目录下，右键选择“Git Bash Here”，输入一下命令：
```cmd
hexo new "filename"
```
这里的filename即文章链接地址，执行成功后进入“source\_posts”目录下就会看到一个以“filename” 命名的md文件，文章内容编辑此文件即可。

# 编辑文章

Hexo博客文章分为两部分，第一部分是文章的属性，第二部分是文章的内容，文章的内容可以参考[**Markdown入门指南**](http://www.jianshu.com/p/1e402922ee32/)。
文件内“---”括起来的部分是文章的属性，具体如下：
```cmd
---
title: #文章标题
date: #文章发表时间
tags:  #标签
	- 标签1
	- 标签2
updated: #更新时间
comments: #是否开启评论（需要配合评论功能，后面会讲）
categories: #分类
	- 分类1
	- 分类2
---
```
comments是否开启评论用true和flase表达。
编辑好内容后直接保存即可。