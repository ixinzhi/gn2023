# 如何用Blender來玩VR

作者：3213213210

TID：27900

<title>1</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 1

首先，你得有HTC Vive、WindowsMR、Fove、Oculus Rift其中一種硬體
然後到 [https://www.marui-plugin.com/blender-xr/](https://www.marui-plugin.com/blender-xr/) 照著說明下載(第一步：下載他的Blender，第二步：下載GitHub裡面的dll檔丟到第一步的資料夾裡)

再來是有了軟硬體以後該作什麼

這個，請參考我之前po的模型資源文
[https://giantessnight.com/gnforum2012/forum.php?mod=viewthread&tid=27778](https://giantessnight.com/gnforum2012/forum.php?mod=viewthread&tid=27778)
打開剛剛載的Blender，打開你要的模型，新增VR視窗，現在你跟女森共處一室了
在戴上頭盔之前，把Render模式換成Eevee(右邊工具列點相機，選單第一個就能調整)、
把Overlay關掉(Viewport右上角有一白一黑兩個圓重疊的圖案按掉)，
打開Render再戴上(Viewport右上角有四個球，點最右邊的，電腦爛就點第三個)
接下來，找到手把上的移動鍵，兩個同時按住以後就能用開合來放大或縮小檢視
瘋狂放大看起來就是巨人了，結案
(stukove的專案檔有點問題，目前還沒找到解決方案)

成品圖......抱歉我剛尻完已經關掉了
總之，有問題請發問
<title>2</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 2

问题是静止的我可以在AI少女里面做出来，问题是要会动的 <title>3</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 3

> [dfggggx 發表於 2020-1-26 21:45](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=423672&ptid=27900)
> 问题是静止的我可以在AI少女里面做出来，问题是要会动的

動畫能作啊 關鍵幀插進去 Gragh Editor開起來 我剛測了VR視窗可以播放沒問題Arhoangle的專案檔打開 把男的刪掉 按播放 剛講的一樣能弄
至於要怎麼自己用Blender作動畫我就沒經驗了 目前只玩過物理模擬
<title>4</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 4

还是AI少女比较现成的动作，而且学新的东西估计要花不少时间了，电脑不知道配置够不够 <title>5</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 5

> [dfggggx 發表於 2020-1-27 21:42](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=423757&ptid=27900)
> 还是AI少女比较现成的动作，而且学新的东西估计要花不少时间了，电脑不知道配置够不够 ...

Eevee沒吃多少效能 看你場景的精緻度吧 (我的情況是連場景都沒搭 拿一個人的模型就在玩了)
Render模式跑不了的話可以開開看Material Preview模式(左邊數來第三個圈) 他就不會管你場景裡的光線 顯卡負荷會比較小
先說我是i7+1060 6g 跑起來沒問題