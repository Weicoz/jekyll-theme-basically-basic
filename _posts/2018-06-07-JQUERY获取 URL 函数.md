### JQUERY获取 URL 函数

设置或获取对象指定的文件名或路径。

*window.location.pathname*

例：http://localhost:8086/topic/index?topicId=361
```js
alert(window.location.pathname); //输出：/topic/index
```

设置或获取整个 URL 为字符串。

*window.location.href*

例：http://localhost:8086/topic/index?topicId=361
```js
alert(window.location.href); //输出：http://localhost:8086/topic/index?topicId=361
```

设置或获取与 URL 关联的端口号码。

*window.location.port*

例：http://localhost:8086/topic/index?topicId=361
```js
alert(window.location.port); //输出：8086
```

设置或获取 URL 的协议部分。

*window.location.protocol*

例：http://localhost:8086/topic/index?topicId=361
```js
alert(window.location.protocol); 则输出：http:
```

设置或获取 href 属性中在井号“#”后面的分段。

*window.location.hash*

设置或获取 location 或 URL 的 hostname 和 port 号码。

*window.location.host*

例：http://localhost:8086/topic/index?topicId=361
```js
alert(window.location.host); //输出：http:localhost:8086
```

设置或获取 href 属性中跟在问号后面的部分。

*window.location.search*

例：http://localhost:8086/topic/index?topicId=361
```js
alert(window.location.search); //输出：?topicId=361
```
#### window.location

属性 | 描述
-- | --
hash | 设置或获取 href 属性中在井号“#”后面的分段。
host | 设置或获取 location 或 URL 的 hostname 和 port 号码。
hostname |设置或获取 location 或 URL 的主机名称部分。
href | 设置或获取整个 URL 为字符串。
pathname | 设置或获取对象指定的文件名或路径。
port | 设置或获取与 URL 关联的端口号码。
protocol | 设置或获取 URL 的协议部分。
search | 设置或获取 href 属性中跟在问号后面的部分。
附上一个关于PHP中服务器变量获取query字符串的各个参数方法：

http://blog.unvs.cn/archives/php-server-url-string.html

