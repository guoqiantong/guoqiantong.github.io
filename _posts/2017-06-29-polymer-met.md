---
layout: post
title: "Polymer-初识"
date: 2016-09-23 12:46:42
categories: Polymer
excerpt: "Polymer 什么是Polymer"
---

* Content
{:toc}

## Polymer是什么？

说polymer之前先说说 现在比较火的bootstrap和angularjs，bootstrap前端框架是基于html，css，javascript，让前端开发更加快捷， 即便是对前端开发不太熟悉的开发人员也可以制作很漂亮的页面，而且网上也有很多bootstrap的主题，可以直接使用，很方便。angularjs前端 js框架，给页面添加数据绑定，当然还有其他功能，这里不细说了。使用起来没什么特别的，就是你想用什么组件就把对应的代码贴到你的页面里就行了，比如下 面的按钮组：

{% highlight ruby %}
<div class="btn-group" role="group">
  <button type="button" class="btn btn-default">Left</button>
  <button type="button" class="btn btn-default">Middle</button>
  <button type="button" class="btn btn-default">Right</button>
</div>
{% endhighlight %}

问题来了，如果我想在这个按钮组添加第4个按钮，并且我这个按钮组已经被10个页面使用，我需要改10个页面！当然你会说，可以在程序里把它做成组件，然后让页面去引用，没错这就是目前常用的解决方案，但问题又来了，这是需要做后台的人员完成的。也就是说它不是一个真正的可重用组件。
 
下面该说说主角了polymer
polymer不是组件库，是帮助前端开发人员，更简单快速地开发可重用组件的"类库"。用polymer开发的组件更像程序开发中“类”的概念，也就是组件是一个类，当页面使用这个组件就相当于实例化这个类。如果这个类发生了变化，那么这个类实例化的对象也会随之改变，这就解决了上面说的问题。这大大增强了前端开发的可维护性。
 
举例说明：1.创建一个组件 hello-polymer.html
![创建一个组件]({{ site.url }}/assets/201609231474610751187996.png)

2.组件引用

![组件引用]({{ site.url }}/assets/201609231474610780845036.png)

图中<hello-polymer></hello-polymer>就是polymer引用组件的方式，是不是很像html标签。
 
polymer官网已经添加很多常用的组件供开发者使用(*[点击访问官方组件](https://elements.polymer-project.org/))，能够满足简单的网站开发。
 
以上内容是本人通过使用polymer后的看法，有不对的地方请指正，想看官方讲解(*[点这里](https://www.polymer-project.org/1.0/))
 
使用polymer的弊端:
1.网上的质料很少，中文的更少，学习成本高。
2.官方组件有限，有些组件还需要自己写。
3.官网网站经常访问不了