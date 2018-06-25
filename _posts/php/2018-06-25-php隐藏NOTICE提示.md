---
layout: post
title: php隐藏NOTICE提示
description: ""
categories: ['php']
modified: 2018-06-25
---

### php隐藏NOTICE提示

{% highlight php linenos %}
<?php
error_reporting(E_ALL || ~E_NOTICE);
error_reporting(E_ERROR | E_WARNING | E_PARSE);
{% endhighlight %}