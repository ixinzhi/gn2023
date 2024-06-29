# 使用泄露的源码在本地部署Novel AI的基本教程

作者：zzh159zzxc

TID：34251

<title>1</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 1

*本帖最後由 juliazhu1978 於 2022-10-9 22:09 編輯*

相信许多坛友最近已经在NovelAI的官网付费尝试了Novel AI作画或者观赏了一些Novel AI作画的图片
那么，有什么办法可以免费且自主的生成Novel AI图片呢？
答案是有的，Novel AI的源码已经流出两个版本，我们可以通过在本地或者私有的服务器部署Novel AI来实现自动生成图片。

一.前提
首先，我们要确保自己持有一张不错的显卡以及充足的内存（RAM）和足够的存储空间。
具体来说，需要一张显存不低于4G的Nvidia显卡，16G RAM，以及最低20G的可自主支配的硬盘存储空间。

二.下载
如果你满足以上需求，可以到以下渠道下载Novel AI的源码，这里给出三种选择
1.精简版和前置内容

https://pan.baidu.com/s/1zDDGbUfXii4ivv68-u80Ug

密码为2zus
B站UP秋叶aaaki制作的精简版，抽掉了一些不必要的模型，基本不影响使用
2.第一版（52G）

1.  magnet:?xt=urn:btih:5bde442da86265b670a3e5ea3163afad2c6f8ecc&dn=novelaileak&tr=udp%3A%2F%2Ftracker.opentrackr.org%3A1337%2Fannounce&tr=udp%3A%2F%2F9.rarbg.com%3A2810%2Fannounce&tr=udp%3A%2F%2Ftracker.openbittorrent.com%3A6969%2Fannounce&tr=http%3A%2F%2Ftracker.openbittorrent.com%3A80%2Fannounce&tr=udp%3A%2F%2Fopentracker.i2p.rocks%3A6969%2Fannounce

*複製代碼*最早流出的版本，也是坛内分享的版本
3.第二版（125G）

1.  magnet:?xt=urn:btih:a20087e7807f28476dd7b0b2e0174981709d89cd&dn=novelaileakpt2&tr=udp%3a%2f%2ftracker.openbittorrent.com%3a6969%2fannounce&tr=http%3a%2f%2ftracker.openbittorrent.com%3a80%2fannounce&tr=https%3a%2f%2ftracker.nanoha.org%3a443%2fannounce

*複製代碼*今天流出的新版本，效果更好但是空间占用更大

三.安装和配置
B站UP秋叶aaaki制作了一个简明的视频教程，可供观看
[https://www.bilibili.com/video/B ... a8d21c2bd43956a4d6e](https://www.bilibili.com/video/BV1aD4y1y7Gg?share_source=copy_web&vd_source=aa367ae96e708a8d21c2bd43956a4d6e)

四.参数的调整
1.Prompt
Novel AI生成图片要依赖用户输入Prompt来指导生成，这里简单介绍Prompt的输入规则
首先，Prompt必须是英语单词或词组，词组中单词的空格由字符“_”代替，例如boots和white_boots
其次，Prompt间需要半角字符“,”来分隔，例如boots,white_boots,white_stocking
第三，可以使用符号“()”和“[]”来增强和削弱某个Prompt的权重，例如（white_boots）,((white_stocking)),[black_boots]

2.Negative Prompt
Novel AI生成图片可以通过输入NegativePrompt来避免生成一些东西，输入规则与Prompt大体一致
这里提供一个示例以为参考

1.  ((lowres)), ((bad_anatomy)), bad_hands, text,error, ((missing_fingers)),extra_digt ,fewer_digits,cropped, wort_quality ,low_quality, jpeg_artifacts,signature,watermark, username, (blurry), (badvfeet), ((((ugly)))), (((duplicate))), ((morbid)), ((mutilated)), (((tranny))), (((trans))), (((trannsexual))), (hermaphrodite), out_of_frame, extra_fingers, mutated_hands, ((poorly_drawn_hands)), ((poorly_drawn_face)), (((mutation))), (((deformed))), ((ugly)), blurry, ((bad_anatomy)), (((bad_proportions))), ((extra_limbs)), cloned_ face, (((disfigured))). (((more_than_2_nipples))). out_of_frame, ugly, extra_limbs, (bad_anatomy), gross_proportions, (malformed_limbs), ((missing_arms)), ((missing_legs)), (((extra_arms))), (((extra_legs))), mutated_hands, (fused_fingers), (too_many_fingers), (((long_neck))), ((((penis)))), ((((dick)))), strong, ((((futa)))),(thick_thigh),((toned_abs))

*複製代碼*3.Sampling Steps
Sampling Steps控制图片的精细程度，一般来讲数值越高图片越精细，生成速度越慢

4.Width和Height
不多赘述，控制图片长宽像素，越大生成时间越久，要求配置越高

笔者的3070Ti Laptop最大生成大小为1280*1280
据报告，生成大小越大，图片更精细的可能性越高

5.img2img
一个自行提供图片来指导生成的功能，除了能自行提供图片外，与txt2txt模式基本一致

<title>2</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 2

感谢！直接把源码搞到确实方便。 <title>3</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 3

好像很不错 回头试试看能不能自己也弄一个 话说楼主感觉显卡压力怎么样 废片率如何 <title>4</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 4

想问一下大佬们，1060的显卡做一张图需要多久呢？ <title>5</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 5

同看到了视频，结果发现电脑没有这个条件QwQ <title>6</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 6

> [wwwnwy 發表於 2022-10-9 21:24](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=517495&ptid=34251)
> 好像很不错 回头试试看能不能自己也弄一个 话说楼主感觉显卡压力怎么样 废片率如何 ...

压力其实还好，3070Ti Laptop在这方面还是很有余裕

废片率大概是在2-3成？

<title>7</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 7

> [juliazhu1978 發表於 2022-10-9 22:03](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=517500&ptid=34251)
> 压力其实还好，3070Ti Laptop在这方面还是很有余裕
> 
> 废片率大概是在2-3成？

那似乎还可以 回头拿我1660来试试

2-3成废片率好像还行 不算高
<title>8</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 8

可惜我硬盘塞满了，不然我高低得整一个来折腾下我的3070ti <title>9</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 9

感谢楼主分享，一直都想尝试AI工程化制图的项目！！！
<title>10</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 10

艹，很详细，有空就拿我的3060整整。感谢楼主！ <title>11</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 11

大佬验证码是不是改了,我死活进不去 <title>12</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 12

话说NAI的强调不是{}吗？（）强调好像是另一个AI的？
<title>13</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 13

楼主麻烦问一下 这个125G的库下好了 应该放在哪里或者替换什么文件才能应用起来？
<title>14</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 14

> dfggggx 發表於 2022-10-9 21:53
> 想问一下大佬们，1060的显卡做一张图需要多久呢？

3070据说七秒就能干一张出来     也许可以参考参考？（