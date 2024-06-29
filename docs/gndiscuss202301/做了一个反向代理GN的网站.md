# 做了一个反向代理GN的网站

作者：AlexYuan

TID：29654

<title>1</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 1

*本帖最後由 AlexYuan 於 2020-10-20 16:56 編輯*

[https://fd.taxuexunmeicloud.top/gnforum2012/forum.php](https://fd.taxuexunmeicloud.top/gnforum2012/forum.php)
通过这个域名就可以不挂代理访问GN了
（目前服务器不太行 会比较慢
过几天换个线路好点的服务器看看

测试了一下发现 跳转页面会有问题。。
比如说 点击【原创文章区】还是会跳转到url为
[https://giantessnight.com/gnforu ... =forumdisplay&fid=7](https://giantessnight.com/gnforum2012/forum.php?mod=forumdisplay&fid=7)
的页面 而不是跳转到
[https://fd.taxuexunmeicloud.top/gnforum2012/forum.php](https://fd.taxuexunmeicloud.top/gnforum2012/forum.php)?mod=forumdisplay&fid=7
10.20更新
已经关闭了反向代理了  因为有些问题没法解决
所有各位还是...继续挂梯子吧
<title>2</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 2

这也太强了...是大佬我死了![](img/eb53e31c2f6d4b3faf8afed7e42e050a.png) <title>3</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 3

唔...为什么我直接404了呢...![](img/afcc6a4838933b8dab98174a1c1bd853.png) <title>4</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 4

> [147c147 發表於 2020-10-11 19:04](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=449737&ptid=29654)
> 唔...为什么我直接404了呢...

因为在调试...跳转不解决的话就没啥用![](img/c21ba2c6b3682f8392e3b81ea4b59fd7.png)
<title>5</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 5

要做GN反代理，需要論壇後台與服務器設定才方便實現。
由於論壇版本較舊，有些頁面上的網址是寫死giantessnight.com/gnforum2012域名的，另外UCenter路徑不同的問題也不好處哩，因此單純的反代理會很難實現。

<title>6</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 6

> [phone2345 發表於 2020-10-11 20:29](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=449749&ptid=29654)
> 要做GN反代理，需要論壇後台與服務器設定才方便實現。
> 由於論壇版本較舊，有些頁面上的網址是寫死giantessn ...

我尝试用内容替换..
替换了
text/html
text/plain
text/css
text/xml
text/javascript
text/x-component
application/json
application/javascript
application/x-javascript
application/xml
application/xhtml+xml
application/rss+xml
application/atom+xml
application/x-font-ttf
application/vnd.ms-fontobject
image/svg+xml
image/x-icon
font/opentyp
但是还是没用。。。
其实不考虑访问速度的话，联系但大再绑定一个域名就可以了...
<title>7</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 7

*本帖最後由 phone2345 於 2020-10-11 20:51 編輯*

> [AlexYuan 發表於 2020-10-11 20:35](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=449750&ptid=29654)
> 我尝试用内容替换..
> 替换了
> text/html

最簡單的方式是申請一個免費域名(freenom)，掛免費反向代理(cloudflare)，然後GN在Ucenter中設定应用的其他 URL，就能實現不同域名自動內容跳轉。不過GN服務器應該還有綁定域名的設定，可能也需要增加回應的域名，不然只會是404。

不過在這麼做之前，得先考慮GN管理是否願意讓論壇主動解除被牆的狀態，畢竟也有用戶的意見是希望持續這個被牆狀態，讓環境單純一點。

<title>8</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 8

> [phone2345 發表於 2020-10-11 20:49](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=449756&ptid=29654)
> 最簡單的方式是申請一個免費域名(freenom)，掛免費反向代理(cloudflare)，然後GN在Ucenter中設定应用的其 ...

确实                                             <title>9</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 9

这个太强大了，是不是可以不用VPN了