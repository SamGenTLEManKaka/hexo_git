
---
title: Hexo从入门到放弃之修改文章底部标签
date: 2017-07-28 08:48:51
tags: 
	- Hexo
	- Node.js
updated:
comments: true
categories: 
	- Hexo
---
> 博客底部tags标签是个“#”号太丑了，想更换一个

<!--more-->
# 前后效果对比

> 更换前样式

![picture](\img\底部标签.png)

> 更换后样式

![picture](\img\tags效果图.png)

#具体实现方法

修改主题根目录下layout/_macro/post.swig文件，搜索 rel="tag">#，将 # 换成<i class="fa fa-tag"></i> 即可
```cmd
<div class="post-tags">
          {% for tag in post.tags %}
            <a href="{{ url_for(tag.path) }}" rel="tag"><i class="fa fa-tag"></i>{{ tag.name }}</a>
          {% endfor %}
        </div>
```