---
layout: post
title: jquery根据name属性查找元素
description: "jquery根据name属性查找元素"
modified: 2018-06-11
categories: ['js']
tags: ['js']
---

### jquery根据name属性查找元素

{% highlight js linenos %}
//选择所有含有id属性的div元素
$("div[id]");

//选择所有的name属性等于'newsletter'的input元素
$("input[name='newsletter']");

//选择所有的name属性不等于'newsletter'的input元素
$("input[name!='newsletter']"); 

//选择所有的name属性以'news'开头的input元素
$("input[name^='news']");

//选择所有的name属性以'news'结尾的input元素 
$("input[name$='news']");

//选择所有的name属性包含'news'的input元素
$("input[name*='man']");

//可以使用多个属性进行联合选择，该选择器是得到所有的含有id属性并且那么属性以man结尾的元素
$("input[id][name$='man']");

{% endhighlight %}