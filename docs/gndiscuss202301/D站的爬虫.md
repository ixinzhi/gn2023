# D站的爬虫

作者：cuitianhaocy

TID：29078

<title>1</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 1

最近在公司实习摸鱼，写了个D站的爬虫（DeviantArt），可以爬OHH,MS等大神的作品，需要的小伙伴自取，可能要一点python基础
<title>2</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 2

 <ignore_js_op>![](img/6c3cc0fc66d1e46ce43643929f01f300.png)

[DevianArt_Spider.zip](forum.php?mod=attachment&aid=ODM5NTJ8YmU4YzZjMjB8MTY3NDA2NjMxMHwxODIzMHwyOTA3OA%3D%3D)

2020-7-15 21:29 上傳

點擊文件名下載附件

8.66 KB, 下載次數: 35</ignore_js_op> <title>3</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 3

非常好，以前用的是github上别人的java（已经废了），一直不会用selenium（懒），谢谢
![](img/04677f683de6ca11476a5d07783b9b0e.png)

一些问题吧
(1) 拿cookie，下载的时候要开全局代理，不过不是什么大问题。
(2) BUG: File: getUrls.py  line 11 : initChrome 函数名错误，注意大写

正在跑测试例，网速挺慢的，估计可行 <title>4</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 4

> Dibdabdu 發表於 2020-7-15 22:30
> 非常好，以前用的是github上别人的java（已经废了），一直不会用selenium（懒），谢谢

哈哈 感谢指正 实现在这个也只能算是半成品 还有很多不完善的地方 <title>5</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 5

*本帖最後由 sidefx 於 2020-7-16 06:42 編輯*

其实不用Webdriver也可以的，直接跳过翻页，效率更高一些吧。
我的理念是javascript能无视就无视比较好 xD

用一个普通的http client直接去发ajax request也是可以的。
可以开一个sniffer看一下browser发了什么样的request，然后照做就行了(目前绝大多数网站还是比较简单)。

新版DeviantArt的列表request格式是类似
“https://www.deviantart.com/_napi/da-user-profile/api/gallery/contents?username=#{username}&offset=#{offset}&limit=#{limit}&folderid=#{folderid}”
这种的，

这个会返回一个json，里面有需要的信息，下载列表里的资源需要用到里面给出的token。旧版的有个"super preview"，
就是不用进页面就直接有最大尺寸的url，新版的还没有仔细看，不过暂时没找到。

最直接的还是request一下列表里的每个页面，然后用里面的token去request那个资源(header里还需要把referer设成对应的页面)。

<title>6</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 6

可以可以，回头去试试