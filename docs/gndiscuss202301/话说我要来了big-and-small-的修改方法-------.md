# 话说我要来了big and small 的修改方法.......

作者：wongvict

TID：733

<title>1</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 1

今天问一个国外的高人，他给我发来了修改big and small的修改方法，（boysgts老兄的求助贴见[http://giantess-night.com/gts_ta ... &extra=page%3D1](http://giantess-night.com/gts_talk/viewthread.php?tid=719&extra=page%3D1)）。但是本人英语水平不高，无法完全理解。哪位高人能给翻译一下啊？
全文如下：
first, find stdrt.exe in C:\Document and settings\(your username)\Local Settings\Temp\mrt*.tmp(* is a hex number) do this while game running.

then copy all the thing in the file(shoulg include stdrt.exe) in somewhere.

also, remember the directory of stdrt.exe and BIG and Small.exe.

then type it into a link:

"directory of stdrt.exe" /SF "directory of BIG and Small.exe" /SO94208

after on you use CE, choose stdrt.exe and 4 bytes.

the important part:

you type 4294967295-the target value instead of typing the target value.

e.g if it is 100 then it would be 4294967295-100=4294967195.

also if the value is lower then 2147483649 it becomes negative value.

then freeze the value(1ms freeze interval recommended, because 1ms is the minimum)

if you got problems, reply me.
谢谢了啊![](img/f04f0b7ab164c5c0e7c50a427ee2773f.png) <title>2</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 2

這個上次討論過，但是我的理解能力是達不到了

你可以用個變速齒輪之類的外掛玩，速度放慢了感覺更爽 <title>3</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 3

恩值得试试，但是估计死得更快了![](img/713872392f0257089685e7800521c504.png) <title>4</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 4

我提出1個基本問題：after on you use CE, choose stdrt.exe and 4 bytes. 這句話裡面的「CE」是什麼？是一種遊戲修改軟體的簡稱嗎？全名呢？

這個解決的話，我想我有辦法修改成功。 <title>5</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 5

CE好像是CHEAT ENGINE的縮寫 <title>6</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 6

我用变速齿轮把猫狐那个下克上的通关了 <title>7</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 7

我試了一個多小時沒試出來
CE是CHEAT ENGINE沒錯
可是你給的步驟中間有段沒交代清楚

the important part:
you type 4294967295-the target value instead of typing the target
then it would be 4294967295-100=4294967195.
also if the value is lower then 2147483649 it becomes negative value.
then freeze the value(1ms freeze interval recommended, because 1ms is the minimum)

這段沒交代清楚我沒辦法
你請他一步一步的跟你說吧 <title>8</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 8

谢谢各位了。我试出来后通知大家。此篇英文版给需要的同志们参考好了 <title>9</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 9

我也失敗，似乎跟Js卡在相同的問題上。那一段跟實際操作似乎搭不太起來。 <title>10</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 10

這之前我也有弄過，但沒有成功。![](img/1751a37041f23d672f2071488c42b774.png) <title>11</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 11

1、運行游戲後會在緩存文件夾下生成一個文件夾，通常為C:\Document and settings\(your username)\Local Settings\Temp\mrt*.tmp,
里面有stdrt.exe程式

2、將此文件夾內容拷入BIG AND SMALL游戲目錄，新建立一個快捷方式如&quot;D:\Game\Big and Small\stdrt.exe&quot; /SF &quot;D:\Game\Big and Small\BIG and Small.exe&quot; /SO94208

3、執行該快捷方式啟動游戲，進入游戲後暫停，記住要修改的數據，比如初始血值為100。

4、打開CHEAT ENGINE，選搜尋進程為stdrt.exe，value type選擇4 bytes。用「4294967295」這個數減去目前的血值「100」，得到「4294967195」這個數。

5、接著搜尋「4294967195」，此時會出現若干結果；再來返回游戲，當生命值變化後（通常是扣血，如扣了兩滴血變成「98」），暫停游戲，切換到CHEAT ENGINE，再次搜尋用「4294967295」減去當前生命值（例如98）的結果。

6、如果此時你得到一個結果，則雙擊改結果，將軟體下方出現的值change value，改成低於2147483649的值，然後鎖定，於是生命值將不再減少。但如果得到仍是複數的結果，則再重復以上步驟（讓生命值繼續扣血，如96，再循環下去……）。

7、同理，可以修改其他數值。 <title>12</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 12

谢谢楼上~~~,修改成功了~~~![](img/04677f683de6ca11476a5d07783b9b0e.png) <title>13</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 13

知道了谢谢！！![](img/f04f0b7ab164c5c0e7c50a427ee2773f.png) <title>14</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 14

哎！！！！！！！！！！！！！！！！！！！！！！ <title>15</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 15

我也修改成功了，非常感謝a大圖文並茂的解釋！ <title>16</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 16

通常為C:\Document and settings\(your username)\Local Settings\Temp\mrt*.tmp “stdrt.exe”可是怎么空啊 我笨啊 要玩~那里教我什么修改方法 请说话！![](img/505c2745f5275f64defe86b0d3b4d98d.png) ![](img/505c2745f5275f64defe86b0d3b4d98d.png)