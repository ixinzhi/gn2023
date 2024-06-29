# 手机实现免梯访问gn的方法(加密DNS)

作者：LTHPKBTE

TID：33533

<title>1</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 1

*本帖最後由 LTHPKBTE 於 2022-6-27 18:37 編輯*

**手机排版可能会导致错乱，如有观感问题非常抱歉**

此方法提供给不想挂梯子 没有root权限修改hosts文件的手机用户。
在使用此方法前请确认手机系统支持设置加密的DNS。目前已经确认MIUI12.5以上版本都支持。

以下提供以MIUI12.5.9版本为例的设置方法:
1.打开设置，找到"连接与共享"点击进入。
2.找到"私人DNS"设置项，点击更改设置。
3.将模式更改为"私人DNS提供商主机名"，在出现的框中填入"dns.google.com"，保存，完成。

注意事项: DNS可能需要几分钟来刷新缓存。尽量不要使用手机自带的浏览器访问站点，推荐via或者Chrome。 <title>2</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 2

![](img/51c9d25d5c87303019ce0d6f9fff3a3c.png)不用gn的时候记得改回去 不然访问国内网站速度会慢一些 <title>3</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 3

大佬强，已经成功了                            <title>4</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 4

哇塞，厉害，这下确实多一条备选路径可以走了。感谢。 <title>5</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 5

林檎手机用户请自行退出（狗头） <title>6</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 6

感谢大佬，收藏一下预防梯子失效 <title>7</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 7

好东西，收藏了，等这个方法失效后就试（ <title>8</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 8

牛逼 改DNS翻墙的原理到底是什么啊 好神奇啊 <title>9</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 9

话说现在能用的DoH的服务器都有啥 <title>10</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 10

*本帖最後由 Foobarz 於 2022-7-11 00:20 編輯*

Android 9 以后的 Private DNS 用的貌似是 DNS over TLS 来着（over HTTPS 大概要到 13 才支持），以及 iOS / macOS 的话要自己添加描述文件才行。
[https://giantessnight.com/gnforum2012/forum.php?mod=viewthread&tid=33656&page=1&extra=#pid509043](https://giantessnight.com/gnforum2012/forum.php?mod=viewthread&tid=33656&page=1&extra=#pid509043)