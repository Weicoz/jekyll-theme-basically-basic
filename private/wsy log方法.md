---
layout: post
title: wsy_log方法
description: ""
modified: 2018-06-25
categories: ['work']
tags: [work]
---

{% highlight php linenos %}
<?
require_once(ROOT_DIR."mp/lib/LogOpe.php");
$log_ope = new LogOpe("file");
$log_ope->log_insert("msg");


//日志记录
$zlog_name = "{$_SERVER['DOCUMENT_ROOT']}/weixinpl/log/filetest_".date("Ymd").".log";//log文件路径
$zlog_time = "\n--- ".date("Y-m-d H:i:s")." ----- LINE:".__LINE__." ----- URL:{$_SERVER['PHP_SELF']} ---------\n";
file_put_contents($zlog_name,"{$zlog_time}",FILE_APPEND);



//日志记录 - 方法版v3
public function zlog_insert($log_name, $log_content, $isclean = 0){
    $debugInfo = debug_backtrace();
    $log_name .= "_".date("Ymd").".log";
    $zlog_name = "{$_SERVER['DOCUMENT_ROOT']}/weixinpl/log/{$log_name}";//log文件路径
    $time = date("Y-m-d H:i:s");
    $content_info = "DEBUG --- time:{$time} --- LINE:{$debugInfo[0]['line']} --- func:{$debugInfo[1]['function']} --- URL:{$_SERVER['PHP_SELF']} ---\n";
    $log_content = $content_info.$log_content;
    //file_put_contents($zlog_name ,$log_content,$isclean ?: FILE_APPEND);
    _file_put_contents($log_name ,$log_content,$isclean ?: FILE_APPEND);
}

/**
 * 服务器端 console
 * @param string $log_content
 * @param string $log_level
 */
public function console_php($log_content = "",$log_level = "DEBUG"){
    include_once ($_SERVER['DOCUMENT_ROOT'].'/weixinpl/common/ChromePhp.php');
    $debugInfo = debug_backtrace();
    \ChromePhp::group("{$this->func} --- LINE:{$debugInfo[0]['line']}");
    \ChromePhp::warn("{$log_level} --- LINE:{$debugInfo[0]['line']} --- func:{$debugInfo[1]['function']}");
    \ChromePhp::log($log_content);
    \ChromePhp::groupEnd();
}
{% endhighlight %}

user_id：302701

openid：oV4YRt4wmo_BNo7HB9ot_2uP_LH4

