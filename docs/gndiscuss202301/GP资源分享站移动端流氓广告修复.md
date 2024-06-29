# GP资源分享站移动端流氓广告修复

作者：狐乐

TID：34014

<title>1</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 1

*本帖最後由 Lcxzyr 於 2022-8-30 22:53 編輯*

前段时间有人和我反应，说GP移动端的广告过于流氓，几乎不能用。当时我给出的解决办法是切换到电脑模式

这两天我仔细检查了一下，从网站层面进行了一个简单的屏蔽，现在GP的移动端网页也可以正常使用了

先说结论：

**GP移动端不再会自动跳转到无法返回的流氓广告页面**
**只有点击按钮或链接时才可能会跳转到广告页面**

简单来说，流氓广告投放者在手机页面上投放了一个弹窗广告，而弹窗广告将用户的浏览器劫持，不让浏览器返回。如果强行快速按返回键，则会进入上一页，导致用户无法进入下级目录（进入下级目录-广告跳转-强行返回-返回到上一页）

现在我通过自行劫持浏览器判断标识，让流氓广告无法识别手机页面而不弹出，这样用户就可以长期的不受强制跳转干扰的停留在某个目录页面

最后

**资源收集不易，二道贩子攻击不停，服务器和存储价格不菲，恳请各位在条件允许的情况下关闭反广告使用本站**
**条件允许的情况下，希望大家能帮我宣传一下本站**

**最后附上GP的地址：[https://share.giantess.eu.org](https://share.giantess.eu.org)**
<title>2</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 2

感谢大佬分享，想问一下，里面的东西怎么下载，那几个游戏我点开后显示403 <title>3</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 3

> [sktggy3 發表於 2022-8-31 00:12](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=514342&ptid=34014)
> 感谢大佬分享，想问一下，里面的东西怎么下载，那几个游戏我点开后显示403 ...

理论上来说应该不会出现403
是只有游戏下载会出现403吗？最好告诉我一下具体是哪个文件无法下载
<title>4</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 4

今天又修复一个内部权限配置不当导致内部拒绝访问的bug，不另外开贴了 <title>5</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 5

哎，真的是感谢大佬辛劳了，那么多的资源整合.. <title>6</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 6

> [Lcxzyr 發表於 2022-8-31 02:37](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=514358&ptid=34014)
> 理论上来说应该不会出现403
> 是只有游戏下载会出现403吗？最好告诉我一下具体是哪个文件无法下载
> ...

就是Escape那个。上面是403下面是该文件不支持预览 <title>7</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 7

我试了试，但是看样子完全用不了呢……

试着点了“Download (ad)”来下载。虽然关闭掉uBlock Origin以后可以看到广告了，但是所有的广告都没法前进。

所以看起来没法下载任何文件的样子。

悲哀呢…… <title>8</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 8

> [狐乐 發表於 2022-8-31 12:44](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=514385&ptid=34014)
> 我试了试，但是看样子完全用不了呢……
> 
> 试着点了“Download (ad)”来下载。虽然关闭掉uBlock Origin以后可 ...

啊！找到解决方案了！

把链接“[https://share.giantess.eu.org/1\. ... F%E7%88%B1%E8%B6%B3](https://share.giantess.eu.org/1.Articles/%E5%94%AF%E7%88%B1%E8%B6%B3)(-2022.4).rar?preview”最后的“?preview”去掉就是直接的下载连接了！
<title>9</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 9

> [sktggy3 發表於 2022-8-31 10:33](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=514376&ptid=34014)
> 就是Escape那个。上面是403下面是该文件不支持预览

啊这个其实不是没法下载

上面这个403是网站自己内部显示东西的错误，无法预览指的是压缩包没法在网页端预览，下载按钮在右下角，是一个下载图标
<title>10</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 10

*本帖最後由 Lcxzyr 於 2022-8-31 14:07 編輯*

> [狐乐 發表於 2022-8-31 12:44](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=514385&ptid=34014)
> 我试了试，但是看样子完全用不了呢……
> 
> 试着点了“Download (ad)”来下载。虽然关闭掉uBlock Origin以后可 ...

虽然但是，Downloadad字样的按钮，写了ad那其实就是一个跳转到广告页面的假下载按钮而已
如果需要下载的话，可以点击右下角的下载按钮
(在文件列表页面时那个按钮的功能是切换列表/网格模式，而且在网格模式下可以预览图片)
<title>11</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 11

> [Lcxzyr 發表於 2022-8-31 13:54](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=514392&ptid=34014)
> 虽然但是，Downloadad字样的按钮，写了ad那其实就是一个跳转到广告页面的假下载按钮而已
> 如果需要下载的话 ...

啊！真的呢！我还以为ad是说看一个广告就可以下载了的意思

右小角的按钮真的可以用诶！