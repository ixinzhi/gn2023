# DigiGirl 模型修改教程

作者：nfsaoc

TID：1786

<title>1</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 1

SB3Utility 修改 DigiGirl 教程:
運行要求:

> Requirements
> ============
> - DirectX v9.0c
> - Microsoft Visual C++ 2008 Redistributable Package (different from the editor)
> - .NET Framework 3.5 SP1 (different from the Compact Framework)
> - If you're still experiencing a crash on start, try installing CEGui Mesh Viewer

SB3Utility 版本至少是 v.0.7.21 !

一、 查看 .pp 包
   打開 .pp 文件包 (补充: 打开文件后还要在左上角 .pp 栏位 **双击** .pp 文件名)
   1\. 確保 Source Format 選中 "Digital Girl"
   2\. 選擇 .xx 文件
   3\. 選 "Img" 查看是哪個模型
<ignore_js_op>![](img/16f36ec5bd7979cf85d554cb9b88bc6b.png)

**inst1.png** *(19.21 KB, 下載次數: 0)*

[下載附件](forum.php?mod=attachment&aid=NTc5OHw3MTk0ZTAyY3wxNjc0MDY5NzQ4fDE4MjMwfDE3ODY%3D&nothumb=yes)

2008-11-5 19:24 上傳

二、 修改
   1.選擇 .xx 文件
   2\. 選擇 Object Tree
   3\. 選擇 SCENCE_ROOT / Frame ( 改這個比較簡單， 改其它的也能達到縮放效果）
   4\. 修改圖中所示 Matrix 的3個參數, （數值要一樣，否則比例會失調！)：　eg. 全改成 2 , 模型放大已被
   5\. 改完，按 Apply 保存當前的 .xx 文件， 重複 第1.步修改其它的 c 開頭的 .xx 文件
   6\. 保存 .pp 文件包
<ignore_js_op>![](img/514088ebd70d0be145d75c6595d31f36.png)

**inst2.png** *(18.91 KB, 下載次數: 0)*

[下載附件](forum.php?mod=attachment&aid=NTc5OXxlYTQxMmY5Y3wxNjc0MDY5NzQ4fDE4MjMwfDE3ODY%3D&nothumb=yes)

2008-11-5 19:30 上傳

三、
   用這個方法，應該都能成功，但不保證都可以修改

注意事项:
* 修改比例后，　模型的色调会不正常，　这就要设置　Lights (DigiTown程序里) ，　共有４个光源可以调节(选择 Source)
　 放大模型，如果放的太大，光线不好调节，因为光源强度有限，整体会偏暗

不明白的，請跟帖
希望但大置頂，以方便查閱

[ *本帖最後由 nfsaoc 於 2008-11-7 23:03 編輯* ] <title>2</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 2

![](img/e165e72abfe717aae40508dc244b1023.png)
總算弄好了， 傳個20K的圖，費了我好長時間 <title>3</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 3

非常感謝教學，我來設置精華區∼∼ <title>4</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 4

不用謝，
很想看看其他人的 DigiGirl 作品![](img/ad72a6c9f8b62059ace9a2cbbf5d6fb0.png)
特別期待但大的![](img/35adb0d55aee4cdf94da5a40b45604d4.png) <title>5</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 5

爬墙过来的,发图在这太麻烦了 <title>6</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 6

谁有兴趣一起编个小故事的 <title>7</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 7

> 原帖由 *nfsaoc* 於 2008-11-5 19:52 發表 [](http://giantess-night.com/gts_talk/redirect.php?goto=findpost&pid=20945&ptid=1786)
> 不用謝，
> 很想看看其他人的 DigiGirl 作品![](img/ad72a6c9f8b62059ace9a2cbbf5d6fb0.png)
> 特別期待但大的![](img/35adb0d55aee4cdf94da5a40b45604d4.png)

會出人命啦，我最近也有連載在進行耶∼∼∼![](img/90d0214aea1faf0a6ff9ace943de46a1.png)

不過我答應各位會試著作作看……

--
有沒有宇宙戰艦內部的背景模型……（被拖走） <title>8</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 8

另外忘了說，其實我一運行SB3Utility.exe，就會出現「應用程式錯誤」然後被踢出來。這是不是需要我另外安裝什麼程式？ <title>9</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 9

忘記說了， 這個是 .Net 的程式![](img/e165e72abfe717aae40508dc244b1023.png) 要先安裝 .Net Frameworks 3.5 SP1 才行
--- readme 里也有寫 :
Requirements
============
- DirectX v9.0c
- Microsoft Visual C++ 2008 Redistributable Package (different from the editor)
- .NET Framework 3.5 SP1 (different from the Compact Framework)
- If you're still experiencing a crash on start, try installing CEGui Mesh Viewer <title>10</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 10

收到，我會再試一下。 <title>11</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 11

电脑里头原来有装 .Net Frameworks，　所以也没注意到
微软的网站有的下，　很慢就是，　可以去找个直接安装版本的 <title>12</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 12

我看我先暫停一下好了……好不容易SB3Utility.exe可以用，卻輪到DigiGirl打不開了＝ ＝

我下了[http://www.megaupload.com/cn/?d=NUCG17FE](http://www.megaupload.com/cn/?d=NUCG17FE)這個版本，

可是用Microsoft AppLocale掛日文、簡中或英文都打不開，點reg.exe也沒用。

之前我有抓到簡中版的DigiGirl，也玩過一兩回，是不同版本會互衝嗎？（總之我現在兩個版本都打不開了……真妙） <title>13</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 13

DigiGirl那里有下的？能告诉下吗？谢谢！！ <title>14</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 14

额。。谢谢但大，嘿嘿！ 有下载的地方了。 <title>15</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 15

这个游戏没有自动动的,我现在期待啥时出人工少女4,能自调身高就好了 <title>16</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 16

虽然能调，但是MM的皮肤都边黑了，到底是怎么回事啊 <title>17</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 17

To 但大:
         我是直接点 Digital Girl Rin (English).EXE ；　不过之前载了个日文版本的, 用 Reg.EXE 有反应, 那个日版的就是 baidu 贴吧上mofile　里的, 这个可以用
To dfggggx :
         教程最后面的注意事项不是说了吗，因为你缩放了比例，模型光源也会受影响，在 DigiTown 里头调下光源就可以了 <title>18</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 18

不行，调了光源完全没有任何改变，MM还是黑得像黑人 <title>19</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 19

你光源拉的不够近啦, 要么你就不要弄太大</ignore_js_op></ignore_js_op>