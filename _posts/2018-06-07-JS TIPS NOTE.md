### JS TIPS NOTE

- #### setTimeout 注意事项
```js
setTimeout("history.go(-1)",3000); //注意必须在执行的方法内加引号，否则会马上执行
```
---


- #### substr 截取字符串
```js
var str="Hello world!";
document.write(str.substr(3,7)); //lo world!

var str="Hello world!";
document.write(str.substr(3));   //lo worl
//substr() 方法可在字符串中抽取从 start 下标开始的指定数目的字符。
```
---


- #### replace 替换实例
```js
var str="Visit Microsoft!"
document.write(str.replace(/Microsoft/, "W3School"))
```
---


- #### select 通过内容选择 option
```js
$("#jie option:contains('" + jie + "')").prop("selected", true);
```
---


- #### JQ监测页面是否到底部 滚动加载 下拉
```js
$(window).scroll(function () {
    if ($(document).scrollTop() + $(window).height() >= $(document).height()) {
        alert("哦哦,到底了.");
    }
});
```
---


- #### 网页无法复制屏蔽右键
```html
<body oncontextmenu=self.event.returnValue=false onselectstart="return false">
```
---


- #### 网页无法复制屏蔽右键
```html
<body oncontextmenu=self.event.returnValue=false onselectstart="return false">
```
---