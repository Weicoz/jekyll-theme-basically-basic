---
layout: post
title: jquery模拟form表单post提交
description: "jquery模拟form表单post提交"
modified: 2018-06-07
categories: ['js']
tags: ['js','jquery']
---


### jquery模拟form表单post提交

{% highlight js linenos %}
/**
 * jquery模拟form表单post提交
 * Created by Steven Guo on 2016/3/22.
 */
define(function(require , exports , module) {

    var myPost = function(url,args){
        var body = $(document.body),
            form = $("<form method='post'></form>"),
            input;
        form.attr({"action":url});
        $.each(args,function(key,value){
            input = $("<input type='hidden'>");
            input.attr({"name":key});
            input.val(value);
            form.append(input);
        });

        form.appendTo(document.body);
        form.submit();
        document.body.removeChild(form[0]);
    }

    module.exports.myPost = myPost;
});

{% endhighlight %}