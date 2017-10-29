---
title: (二)Hexo从入门到放弃之部署至github page
date: 2017-02-07 08:33:11
tags: 
	- Hexo
	- github
	- github page
	- Node.js
updated:
comments: true
categories: 
	- Hexo
---
> Hexo是搭建好了，但是本地搭建自己YY是绝对不能满足需求的，我们需要把网站部署到公网上，供所有人浏览。可选的方案是使用云主机的方式来发布，这里我们选择成本更低廉的github page部署方式。

<!--more-->
# 前期准备
1、 github账号
[**github账号注册**](https://github.com/join?source=header-home)地址注册github，如果已有github账号，直接使用即可

# Hexo部署至github page
1、登录github
[**github首页**](https://github.com/)，选择“**New repository**”新建项目仓库，在“**Repository name**”里输入：“**YourName.github.io**”这里的“**YourName**”一定要和前面的“**Owner**”里的内容一致，也就是一定要已记得用户名+.github.io命名。
2、复制项目链接
进入刚才新建的项目页面，复制“**Clone or download**”里的https链接，如果找不到，可以直接用这个地址，https://github.com/YourName/YourName.github.io.git ，把链接里的YourName更改为你的用户名即可。
3、修改Hexo配置
进入Hexo根目录，找到一个_config.yml的文件，右击使用notepad++，或者Sublime Text打开（千万不要使用notepad！千万不要使用notepad！千万不要使用notepad！），进入文件的最后一行，看到内容是这样的：
```cmd
deploy:
  type: 
```
添加一些配置信息进去（其中的YourName仍旧改成你的github用户名）：
```cmd
deploy:
  type: git
  repo: https://github.com/YourName/YourName.github.io.git
  branch: master
```
(PS:注意缩进和冒号后面的空格必不可少！)

4、发布Hexo到github page
修改后关闭保存文件，在Hexo根目录右击鼠标，选中“Git Bash Here”，输入命令：
```cmd
hexo g
```
小等一会后继续输入：
```cmd
hexo d
```
如果出现Inof并且没有报错就说明发布成功了，这时候可以通过github page的默认地址：https://YourName.github.io/ 来访问了（YourName依旧换成你的github用户名）
网页生效可能会有几分钟的延迟，没有即时生效不要着急，小等一会即可

[**点此访问**](https://github.com/SamGenTLEManKaka/SamGenTLEManKaka.github.io)我的GitHub