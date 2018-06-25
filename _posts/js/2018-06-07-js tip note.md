---
layout: post
title: js tip note
description: "js tip note"
modified: 2018-06-11
categories: ['js']
tags: ['js','jquery']
---
### js tip note

- #### setTimeout 注意事项
{% highlight js linenos %}
setTimeout("history.go(-1)",3000); //注意必须在执行的方法内加引号，否则会马上执行
{% endhighlight %}
---


- #### substr 截取字符串
{% highlight js linenos %}
var str="Hello world!";
document.write(str.substr(3,7)); //lo world!

var str="Hello world!";
document.write(str.substr(3));   //lo worl
//substr() 方法可在字符串中抽取从 start 下标开始的指定数目的字符。
{% endhighlight %}
---


- #### replace 替换实例

{% highlight js linenos %}
var str="Visit Microsoft!"
document.write(str.replace(/Microsoft/, "W3School"))
{% endhighlight %}
---


- #### select 通过内容选择 option

{% highlight js linenos %}
$("#jie option:contains('" + jie + "')").prop("selected", true);
{% endhighlight %}
---


- #### JQ监测页面是否到底部 滚动加载 下拉

{% highlight js linenos %}
$(window).scroll(function () {
    if ($(document).scrollTop() + $(window).height() >= $(document).height()) {
        alert("哦哦,到底了.");
    }
});
{% endhighlight %}
---


- #### 网页无法复制屏蔽右键

{% highlight html linenos %}
<body oncontextmenu=self.event.returnValue=false onselectstart="return false">
{% endhighlight %}
---


- #### 网页无法复制屏蔽右键

{% highlight html linenos %}
<body oncontextmenu=self.event.returnValue=false onselectstart="return false">
{% endhighlight %}
---