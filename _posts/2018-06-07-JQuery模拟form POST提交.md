### JQuery模拟form POST提交
```js
/**
 * JQuery模拟form POST提交
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

```