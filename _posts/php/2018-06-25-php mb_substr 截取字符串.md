---
layout: post
title: php mb_substr 截取字符串
description: ""
modified: 2018-06-25
categories: ['php']
tags: ['php']
---

### php mb_substr 截取字符串

{% highlight php linenos %}
<?php 
$str='脚本之家：http://www.jb51.net'; 
echo mb_substr($str,0,4,'utf-8');//截取头5个字，假定此代码所在php文件的编码为utf-8 
?> 
{% endhighlight %}