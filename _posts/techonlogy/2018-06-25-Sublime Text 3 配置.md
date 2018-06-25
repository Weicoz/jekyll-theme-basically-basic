---
layout: post
title: Sublime Text 3 配置
description: ""
modified: 2018-06-25
categories: ['techonlogy']
tags: ['techonlogy']
---

### Sublime Text 3 配置

#### 三、配置
点击preferences－setting user，个人设置如下：

{% highlight ini linenos %}
{
    //字体大小
    "font_size": 13.0,
    //字体类型
    "font_face": "mononoki","Consolas",
    // 设置每一行到顶部，以像素为单位的间距，效果相当于行距
    "line_padding_top": 2,
    // 设置每一行到底部，以像素为单位的间距，效果相当于行距
    "line_padding_bottom": 2,
    // html和xml下突出显示光标所在标签的两端，影响HTML、XML、CSS等
    "match_tags": true,    
    // 是否显示代码折叠按钮
    "fold_buttons": true,
    // 代码提示
    "auto_complete": true,
    // 默认编码格式
    "default_encoding": "UTF-8",
    // 左边边栏文件夹动画
    "tree_animation_enabled": true,
    //删除你想要忽略的插件
    "ignored_packages":
    [
        "Vintage",
        "YUI Compressor"
    ]
}
{% endhighlight %}


#### 四、快捷键
1. F11和Shift+F11进入全屏免打扰模式

1. Ctrl+L：选择整行，按住继续选择下一行

1. Ctrl+KK:从光标处删除至整行的尾部

1. Ctrl+Shift+D:复制光标所在的整行，插入在该行之前

1. Ctrl+J：合并行(已选择需要合并的多行时)，可以理解为不换行模式，直到遇到编辑器边框后自动换行

1. Ctrl+D:选词，(按住-继续选择下个相同的字符串)

1. Ctrl+/：注释整行，可来回切换，Submlie Text可自动判断文件类型。选择整段，也可注释整段。

1. Ctrl+Shift+/:注释。选择整段，也可注释整段，单行时候，不注释该行，而是添加该行的注释信息，如\<!--  -->

1. Alt+. ：闭合当前标签

1. Ctrl+Shift+[：折叠代码

1. Ctrl+Shift+]：展开代码

1. Shift+table:向左缩进、Tab向右缩进
