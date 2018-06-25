---
layout: post
title: HTML TIPS NOTE
description: ""
modified: 2018-06-25
categories: ['html+css']
tags: ['html','css']
---

### HTML TIPS NOTE
- #### HTML 空格

{% highlight html linenos %}
&nbsp;
{% endhighlight %}

---

- #### 提高优先级 !important

{% highlight css linenos %}
.css{color:#fff !important}
{% endhighlight %}

---


- #### CSS文字过长自动省略号

{% highlight css linenos %}
white-space: nowrap;
text-overflow: ellipsis;
overflow: hidden;
{% endhighlight %}

---


- #### CSS a标签无效

{% highlight css linenos %}
a{pointer-events:none;}
{% endhighlight %}

---


- #### IE上运行firebug

```html
<script type="text/javascript" src="https://getfirebug.com/firebug-lite-debug.js"></script>
```

---


- #### IE7 display:inline-block

- 第一种：专门为IE7写Hack

{% highlight css linenos %}
display:inline-block;
*display:inline;
*zoom:1;
{% endhighlight %}

特别是 ZOOM:1 这个必须的
- 第二种：

{% highlight css linenos %}
.selector { display: inline-block }
.selector { *display: inline }
{% endhighlight %}

---

- #### Chrome Hack

{% highlight css linenos %}
@media screen and (-webkit-min-device-pixel-ratio:0) {
    .iProduct_img .iimg img{width: auto;}
}
{% endhighlight %}

---