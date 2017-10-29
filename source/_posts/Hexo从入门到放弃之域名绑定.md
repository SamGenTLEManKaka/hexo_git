---
title: (五)Hexo从入门到放弃之域名绑定
date: 2017-07-15 16:41:50
tags: 
	- Hexo
	- github
	- 万网
	- Node.js
updated:
comments: true
categories: 
	- Hexo
---
> 不愿意用github的二级域名，就申请自己的域名来解析

<!--more-->
# 万网域名+DNS
1、域名的申请就不占用篇幅了
2、解析需要把自己的域名解析到自己的github空间上，一共需要加三条记录如图是我的添加纪录
![picture](\img\解析.png)

# github配置
1、第一种方法是在Hexo根目录下的public\目录新建一个名为CNAME的文件（没有文件类型后缀，如果后，请删除），用记事本打开，里面写上你自己的域名（http部分不需要写）
例如我就写：gentlemankaka.com
然后重新发布下Hexo即可
```cmd
hexo g
hexo d
```
2、第二中方法是去github你的项目页面，点击settings进入设置页面，然后找到Custom domain配置项，把你的域名填写进入即可（同样http部分不写）