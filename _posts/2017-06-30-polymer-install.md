---
layout: post
title: "Polymer-安装"
date: 2016-09-23 14:08:52
categories: Polymer
excerpt: "Polymer 什么是Polymer"
---

* Content
{:toc}

**使用Bower安装**

为项目添加bower.json
{% highlight ruby %}
bower init
{% endhighlight %}
 
## 安装Polymer
 
安装最新版本的Polymer
{% highlight ruby %}
bower install --save Polymer/polymer
{% endhighlight %}
安装指定版本的Polymer
{% highlight ruby %}
bower install --save Polymer/polymer#^1.4.0
{% endhighlight %}
 
## 更新Polymer
{% highlight ruby %}
bower update
{% endhighlight %}
 
**Zip包安装**
Polymer官网可以下载zip包直接使用，适合初学者使用，不需要任何工具，下载后就能使用，因为官方下载地址经常访问不了。
 
polymer：核心文件
webcomponentsjs：[什么是webcomponentsjs?](http://sentsin.com/web/1089.html) 简单点说，就是使组件独立，不受其他组件和代码干扰的标准。目前这种标准还没有应用于所有浏览器，所以还需要手动添加。