# 個人archive和支持的站點説明

作者：sidefx

TID：28566

<title>1</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 1

最早就是看到聊天群裏時不時會有人求一些作者刪掉的圖，產生了這個想法。這幾天看到別人的帖子又想起來了。

手工備份比較費時費力，不過我這裏很多網站的抓取都實現過，像Twitter，DeviantArt，ニコニコ静画，或者Fantia。

總覺得直接放Git不太好，因爲可能會造成超出想象的影響。
除了用的人多了對於站點的負擔，就是關於privacy。
(比如Twitter一直在强調用戶内容erasable，去archive的人太多就會破壞這一點，之前有做過Twitter archive的網站都被Twitter告了。)

所以換個形式吧：
在某個網站如果有想要收的用戶id/圖集/tag，在我這裏回復一下或者私信我就好了，然後我去收。
一次貼一個列表，或者把你的整個following頁面直接貼上來也可以。
(本來想做成全自動，就是只要在我的帖子後面按指定格式回復，我的賬戶看到了就會添加job到queue裏，完成以後自動回一個"job done"，不過好像沒那個必要呢，而且這邊工作也比較繁忙___)

這樣就可以保證網上的内容不至於絕版，然後需要看的時候再找我要就好了。
4chan上面類似“XXX又nuke了他自己的賬戶”或者“XXX又被封了”這樣的標題已經見得太多了。
如果是被封的，很多時候作者自己都沒備份，所以有時候發現作者被封以後會第一時間把之前收的文件還給他 XD

目前支持的一部分站點：

Twitter             [用的是老代碼，因爲目前還可以靠改header强制舊UI，不過以後如果這方法失效，就會需要花點時間修復]
                       [理論上包含所有圖片和視頻，但是Twitter的timeline有時會斷，不去看一下是發現不了的]
                       [斷timeline的有一部分情況可以恢復出來]
Pawoo
Facebook
Plurk
新浪微博

Discord             [網上現成的那個很難用，因爲會先在内存裏生成網頁而不是直接把json和附件存下來，太長的話内存就會滿]

Fantia
Enty      
Patreon             [时不时Patreon更新，api改變或者加入新的防bot機制，就需要改些东西才能正常工作]
(當然，這幾個用我的cookie沒法收別人訂閲的内容。)

DeviantArt          [自從更新了之后，access频率太高就会403，时不时需要待机一会]
ニコニコ静画
ニコニコ 3D
Pixiv                [如果量不大的話，這個和Fanbox直接用現成的PixivUtility就行了]
                      [然後，其實PixivUtility改幾句就可以并行]
Nijie                [和上面差不多]
Tinami

Sankaku Complex     [频率太高会403]
                              [另外，這網站目前用特殊方法還能看到被ban的tag，不過可能以後會被patch掉]                    

Pixiv Sketch
Booth               [這個可能除了我以外沒人需要了，就是備份一下商品列表裏的文字和圖片]

ExHentai            [有限流]
NHentai             [無限流]
各种Booru

Tumblr              [如果是被ban的NSFW需要靠Tumbex]

還有些之前有實現但是待修復的，像Pinterest或者Tumbex，因爲用得不多，坏了以後也一直沒有去管。

正常情況下，加一個站點也很快，但是有些網站實現起來比其他的麻煩很多：
Ajax的有時候會很麻煩，還有時可能需要對付reCaptcha。

然後就是關於生放送，
主要是NicoLive Timeshift和FC2，
之前寫了一下這兩個的Streamlink plug-in。
(除了這兩個以外的像Twitch, Picarto, Pixiv Sketch這些的plug-in，Streamlink是自帶的。)
如果有感興趣的作者也可以在我這裏回復一下，
然後我可以加到錄制列表裏。
(如果是常見的，很可能已經在列表裏了，比如寺田さん。)

<title>2</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 2

楼主真的是实干派![](img/ec942b6b7db075eaad5da7a4ad136d51.png)
一样的想法曾经考虑过，也写过一些，发现维护起来太麻烦就放弃了
再次敬佩楼主并感谢楼主为大家所做的奉献~ <title>3</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 3

刚入门编程的小白想问一下，想要破解fantia，pixiv这类站点的收费可见图片，难度有多大？ <title>4</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 4

> [dfggggx 發表於 2020-4-26 08:20](https://giantessnight.cf/gnforum2012/forum.php?mod=redirect&goto=findpost&pid=434499&ptid=28566)
> 刚入门编程的小白想问一下，想要破解fantia，pixiv这类站点的收费可见图片，难度有多大？ ...

因为我并不是做信息安全或者网络这方面的，我能做的基本只是看到谁把前台逻辑漏洞公布出来了，拿去用一下这种程度。
像是以前老Twitter有过”强制follow“，老discuz有过"下载附件不用积分"这样的。
Fantia和Pixiv目前还没有见过人报出来可以越权的前台漏洞(即使是给钱才说的也没见过)。

要直接看到隐藏的内容，除了利用别人找出来的越权漏洞，就只能攻破server了，这个难度比较大。
(根据具体情况可能犯法可能不犯法，不过我觉得做这种的性质和利用跨站脚本偷别人密码已经差不多了)。

(网上肯定有人能做得到，像上回有个人在某个交易网站开张的第一天就攻破了。
还是不推荐，因为这圈子里真的什么人都有。)

个人即使能做到也不会去做吧，毕竟gts圈子本来就不大。特别是对新人作者，有时候多一两个支持都是很大的鼓励呢。
如果只是想练手的话倒是可以试试，可以先把Kali Linux上的工具都看一下，试着probe一下。
然后比起工具，思路更重要吧，可以看看别人的流程，试着理解一下他是怎么从前一步想到下一步的。

<title>5</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 5

大佬nb，这是造福人群啊 <title>6</title> <link href="../Styles/Style.css" type="text/css" rel="stylesheet">

# 6

其實挺早以前就應該做這個事情了。

看到別人求某個刪掉的資源，很多時候我這裏有備份，但是也有時沒有，就會覺得 ”之前早點知道這個作者就好了呢“。