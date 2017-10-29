---
title: Hexo从入门到放弃之博客页尾广告去除
date: 2017-07-16 21:04:13
tags: 
	- Hexo
	- Node.js
updated:
comments: true
categories: 
	- Hexo
---
> 网页的页尾可以发现存有Hexo特有的广告宣传，虽然是开源免费使用的产品，但我还是想把广告去掉

<!--more-->
# 删除页尾广告
博客页尾可以看到如下Hexo的广告
![tupian](\img\页尾.png)
需要到主题配置目录下的layout\_partials目录下（不同主题路径可能会有不通，我这里用的是Next主题）找到footer.swig文件，右键notepad++打开
```cmd
<div class="powered-by">
  {{ __('footer.powered', '<a class="theme-link" href="https://hexo.io">Hexo</a>') }}
</div>

<div class="theme-info">
  {{ __('footer.theme') }} -
  <a class="theme-link" href="https://github.com/iissnan/hexo-theme-next">
    NexT.{{ theme.scheme }}
  </a>
</div>
```
上面的配置就是博客页尾显示的内容，我们把内容更改为自己想要的信息就可以了，下面是我更改后的内容
```cmd
<div class="powered-by">
  {{ __('footer.powered', '<a class="theme-link" href="https://github.com/SamGenTLEManKaka">绅士</a>') }}
</div>

<div class="theme-info">
  {{ __('footer.theme') }} -
    技术成就梦想
  </a>
</div>
```
