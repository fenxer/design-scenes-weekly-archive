# Scenes Weekly #36

2021-12-27

\> 圣诞快乐。这里依然设计视角下的世界——

第 35 期请[在此查看](./Scenes Weekly #35.md)。

本期出现：Apple Product Bezels、北京地铁、 Incoggo、Swift、Open Subscription Platforms、Aftertext、Artist statement generator、Material Design Award Winners 2021、It’s Nice That、chartr.co、Baymard、The MIT Press Reader、meme、TDesign、JFC、Neal.fun

如有格式异常建议点击最上方「在浏览器中访问」。

---

# 微博

1、上周 Apple Design Resources 更新了几个产品的 mockup 模型（Product Bezels）。顺便看了一眼 Facebook 设计团队出品的 Devices 只更新了 iPhone 13 系列产品。但 Apple 将这些 PSD 采取 dmg 封装，可以说是刁难的很明显了。

![b60def8bd5d048c0889e94e559e32fa7.png](Scenes%20Weekly%20%2336.assets/b60def8bd5d048c0889e94e559e32fa7.png)

{上图：所有可用的产品模型}

→ 存储备用

[Apple Design Resources](https://developer.apple.com/design/resources/)

---

2、北京地铁更新了一套新的指示标识，我在微博转发的是讲其中拼音的改动（比如管庄 Guɑ̌nzhuɑng）。而我自己线下实际观察体验：

颜色饱和度更高，大多地铁候车环境是非自然光线照明，使得整体比之前更鲜明。

字体方面，以 10 号线为例（有些站点还是旧设计），首先站名由原来带有喇叭口的黑体，变为了简洁大方的华康金刚黑（以原微博图中字样为例）。然后原本拼音是全大写 uppercase 样式，现在改为首字母大写的标题式写法，错落有致，更加易读。

另外一个很多人发现的细节：拼音中小写字母 a 和 g 是 single-storey 的，到英文都变为 double-storey，没有像之前混用。

![6179199b44bc48109e4712a4a32f0458.png](Scenes%20Weekly%20%2336.assets/6179199b44bc48109e4712a4a32f0458.png)

{上图：一些地铁站点的新标识}

→ 原微博

[https://weibo.com/1419044843/L7mFEEIhX](https://weibo.com/1419044843/L7mFEEIhX)

---

# 摘录

> 今天，酸性设计已经成为欧美右翼提倡的资本主义加速的工具：利用新技术解决目前的资本主义的危机。在这种情况下，这种「看似反叛」的视觉风格受到同样右翼自 由意志主义推动的比特币、Web3、区块链、NFT 等科技资本的欢迎，也就理所当然。当然对完全被俘虏的酸性图形而言，比如 [Uniswap 的形象](https://uniswap.org/blog/brand-update)，它的「酸性」特质已降低了许多。然而这一妥协也可能就是酸性图形的未来。 酸性图形制造出了标新立异的视觉形式，但这种形式的生产方式却是最妥协、最不愿意反抗的。它打出的反抗和批判的幌子，假以时日也一定会因为无法满足视觉符号的消费链条而变得过时和老旧，届时将会有更妥协、更直白、更有奇观冲击力、更不想反抗、更蛊惑人心的视觉 形式出来替换它。

—— The Type T40

---

# 杂事

1、上周 Incoggo 在 Product Hunt 上夺得 Product of the Week 引起了一些争议。Incoggo 是一个可绕过主流媒体付费墙（paywall）的本地代理应用，像 WSJ、NYT、Bloomberg、The Atlantic、Wired等十多家媒体都可以绕过订阅机制直接阅读文章。争吵的评论区分为这么几类画像，一是单纯不想花钱；二是讨厌铺天盖地的订阅制；三是秉持信息共享自由；四是反对这一做法，认为这与偷窃无异——可以看出，一二三画像组成的复杂用户和第四点组成的用户相互对立。

![截屏2021-12-22 15.36.28.png](Scenes%20Weekly%20%2336.assets/%E6%88%AA%E5%B1%8F2021-12-22%2015.36.28.png)

{上图：Incoggo 的 PH 界面}

首先开发者拿 Adblocker 对比，认为自己是付费墙的 blocker。这个概念偷换的有些问题，聚合器时代广告是与平台、创作者所围成一起的价值环链，而广告被屏蔽的是其背后的带有大量隐私标识的数据。广告主想要吸引自身所在利基市场的潜在客户，使之认识到自己品牌的价值——形式不变换个主体来看，想要吸引订阅增长的创作者也是同理。屏蔽广告不会切断价值链，但是会剧烈影响价值链的维度，也是目前互联网下一个内容创作形式进化所趋。但是屏蔽订阅则是对在线支付工具发展的漠视与乌托邦般的理想跃进。

而对于媒体而言，就像原评论中 Roy G. Biv 所说，Incoggo 此举不会增加任何新闻革新的火星。而新闻媒体的革新又与复杂的意识形态挂钩，这显然是一个独立应用所无法波及的层面。「毕竟记者也要吃饭的」。而讨厌新闻业的订阅机制”click to subscribe, call to cancel”也是另一方面的事情了，更何况美国联邦贸易委员会将会[出手治理](https://www.niemanlab.org/2021/11/the-end-of-click-to-subscribe-call-to-cancel-one-of-the-news-industrys-favorite-retention-tactics-is-illegal-ftc-says/)这一遗诟机制。

顺便一提，这个应用会调用本地 Socks 5 代理，和「常用代理应用」冲突。开发者自己声称流量只是途径本地代理没有上传到第三方服务器上，只会获取一些匿名数据。而且我更奇怪 PH 平台是持有怎样的观点去审核该应用上架的。

→ 吃瓜原网站

[Incoggo - Product Information, Latest Updates, and Reviews 2022 | Product Hunt](https://www.producthunt.com/posts/incoggo)

---

2、一篇分析 iOS 15 中内置应用 Swift 使用情况的文章，只要一个二进制文件包含 Swift 就算上。

![ChartBinariesUsingSwift.png](Scenes%20Weekly%20%2336.assets/ChartBinariesUsingSwift.png)

{上图：从iOS 8.0.4 的0行Swift 到 iOS 15.0 的 607 个 Swift 和  114 个 SwiftUI 二进制文件}

这也跟逐个版本增加的二进制文件数量有关系（原作者并没有给出每年的百分比），时至 iOS15，Object-C 依然是核心（89%）。

→ 更多数据

[Apple’s use of Swift and SwiftUI in iOS 15](https://blog.timac.org/2021/1219-state-of-swift-and-swiftui-ios15/)

---

3、Open Subscription Platforms 是一个试图完善订阅平台数据转移标准的组织。我们知道，Substack 和 Ghost 等是可以随时导出自己的个人订阅数据，Medium、 Patreon以及微信公众号（并没有在影射什么）等都是封闭的，对平台有强依附性，无法转出全部订阅者信息。后者有自己的商业考量，但是前者才是以创作者为中心的平台。

**The future is open.**

→ 查看更多开放订阅平台

[Open Subscription Platforms](https://opensubscriptionplatforms.com/)

---

4、不管是 HTML、BBCode 还是 Markdown，都是一种**嵌入式**标记语言，各种与文本本身无关（只与格式有关）的符号充斥在字里行间。那么有没有一种并行式的标记语言，来区分文本和样式呢？Breck Yunits 做一个非常有意思的实验——**Aftertext**。

比如：

```other
- markdown
 I like **newsletter**.
 You can try [zhubai](https://zhubai.love/).
```

用 Aftertext 语法写就是：

```html
- aftertext
 I like newsletter.
 You can try zhubai.
 bold newsletter
 link https://zhubai.love/ zhubai
```

然后通过编辑器的格式优化，可以轻松地只复制粘贴纯文本。独立的样式也适合协作与版本控制，包括声明一些全局的样式，或者引入一些现有的样式库。事后还可以在并行样式里对 AI 训练并智能完成样式控制任务……但同样缺点依然很多。一个很明显的问题是，一个段落中多个相同词汇怎么处理。Breck 引入数组去查询和定位，但是越长的文本会带来越多的成本，即便编辑器可以优化显示这些单词的定位。还有如何去有效区分标记语言与文本语言？现在只是换行识别到头部词汇去渲染。

```html
- aftertext
 Bold it!
 bold it
```

以及 HN 评论中所提及的一种情况：

```other
- plain text
 *I* did not say that.
 I did not say *that*.
```

Markdown 如此普及以至于他可以融入原文本视作一种「语气」，Afertext 的纯文本就无法做到这个了。

事实上并行式标记语言早在1997年就有人提出，后面的几个方案也都非常冗杂。但无论如何，这些对立于现有事物的想法，都是珍贵的思维实验，更别说有一定的实践性了，写完上面这段文字后我依然感到 Aftertext 很有趣。

→ 查看原文

[Aftertext](https://breckyunits.com/aftertext.html)

→ Playground

[Try Scroll - The extensible alternative to Markdown](https://try.scroll.pub/#url%20https://raw.githubusercontent.com/breck7/breckyunits.com/main/aftertext.scroll)

---

5、艺术家声明生成器，为你的艺术自动生成一段博古通今的文案。可生成长中短三种篇幅。之前我应该是看过这个网站，但是最近看到又有人提前。因为太有意思所以就分享出来了。

![截屏2021-12-24 17.33.13.png](Scenes%20Weekly%20%2336.assets/%E6%88%AA%E5%B1%8F2021-12-24%2017.33.13.png)

{上图：生成的一例文本：我的作品探索了包豪斯共情与足球圣歌?的关系，并受到了克尔凯郭尔和弗朗西斯培根的影响BLABLA……}

→ 生成

[Instant artist statement](https://www.artybollocks.com/generator.html)

---

6、这一周开始，各种年终总结都来了。

首先是上周忘记发的 Material Design Award Winners 2021。3M 的那个便签应用 Post-it 拿到了最佳动效，我记得它曾在 2019 年就拿过 Google Play Best Apps。大屏适配应用给了 Todoist ，深色模式奖给了 Meetly。

![meetly.png](Scenes%20Weekly%20%2336.assets/meetly.png)

{上图：Meetly 深色模式界面}

从上图 Meetly 界面中能看到很多 Material Design 元素，这也是入选 MD 奖项的重要因素之一。

→ 详见

[https://material.io/blog/mda-2021-winners/](https://material.io/blog/mda-2021-winners/)

---

7、It’s Nice That 的总结分为了年度 Top 50阅读数、Top 25推荐内容、新闻、插画、平面设计、摄影和访谈。

→ 查看全部总结

[From NFTs to balloon art, we look back on a sometimes chaotic but always creative 2021](https://www.itsnicethat.com/features/review-of-the-year-2021-introduction-creative-industry-201221)

这其中 Elliot Ulm 的作品我尤其喜欢——Elliot 的表达能引起共鸣，是我理想中的表达先于版式的范例。

![Elliot.png](Scenes%20Weekly%20%2336.assets/Elliot.png)

{上图：Elliot Ulm: BYDAYBYNIGHT (Copyright © Elliot Ulm, 2021)}

相反 Gumroad 的新设计就有一种版式先于表达的刻意感。

→ 查看更多 Elliot 作品

[Elliot Ulm’s graphic design memes will make you laugh and then make you think](https://www.itsnicethat.com/articles/elliot-ulm-graphic-design-250521)

---

8、其他年度总结：

经常阅读本通讯的读者应该不陌生 [chartr.co](http://chartr.co) 这个专注数据可视化的 newsletter。2021年他们做了288个图表，现在用其中标志性的25个事件重新回顾下今年。

→ 点此回顾

[https://www.chartr.co/year-in-charts/2021-in-charts](https://www.chartr.co/year-in-charts/2021-in-charts)

专注电商体验量化的 Baymard 的年度总结：

→ Baymard: 2021 and 2022

[Baymard: 2021 and 2022](https://baymard.com/blog/2021-and-2022)

The MIT Press Reader 的总结：

→ 一年内最受欢迎的文章

[Best of 2021 | drugs, translation, consumerism, and more](https://mailchi.mp/mit/best-of-2021?e=%5BUNIQID%5D)

---

9、看个meme休息一下。

![FHJKiUcXoAodeC1.jpeg](Scenes%20Weekly%20%2336.assets/FHJKiUcXoAodeC1.jpeg)

{上图：web1 web2.0 web 3 趋势样式上的区别}

→ 出处

[登录 Twitter，关注jordan singer](https://twitter.com/jsngr/status/1473322154091585537?s=21)

---

10、TDesign 是来自腾讯内部近 300 名设计师与开发者共同打造，经由 500+ 项目使用、验证和锤炼过的企业级设计体系， 秉承包容、多元、进化、连接的价值观，TDesign 期望与用户、行业及合作伙伴等一起打造具有竞争力的产品体验。

[腾讯开源企业级设计体系 TDesign](https://mp.weixin.qq.com/s/aje8auQ2kY8C0pxNUzEV9w)

[上周](./Scenes Weekly #35.md)提到的 TDesign 正式公开，并分为了桌面端、移动端和小程序三部分。其中小程序的文档明显要比微信那边的更具设计亲和力。

![tdCover.png](Scenes%20Weekly%20%2336.assets/tdCover.png)

{上图：TDesign 移动端组件库 Figma 封面}

---

11、日本政策金融公库会发布一些刊物报告，其中国民生活事业相关的一份报告，对餐厅的食物拍照成像效果也做了一些探索。比如搭建半逆光的摄影环境、拍摄角度、还有柔光的应用等面向一般群众的摄影小技巧。

![JFC.png](Scenes%20Weekly%20%2336.assets/JFC.png)

{上图：写真の撮り方ガイド 飲食店編}

由于里面内容不允许随意转载，可直接查看下方文档。

→ 文档（PDF）

[https://www.jfc.go.jp/n/findings/pdf/phototech_guide_restaurant.p](https://www.jfc.go.jp/n/findings/pdf/phototech_guide_restaurant.p)

---

12、Neal.fun 是 Neal Agarwal 做的一个网页小游戏/工具集合，里面还有几年前流行的「如何花XXXX的钱」，最新的一个小游戏是如何在海边叠石头……

→摸鱼放松

[Neal.fun](https://neal.fun/)

---

# 劳逸

![11b56aaafe4342e982bff79f6e020d59.png](Scenes%20Weekly%20%2336.assets/11b56aaafe4342e982bff79f6e020d59.png)

{上图：Bean and Nothingness 横幅}

Bean and Nothingness 这款解谜游戏基于网格和回合制，捡起豆子，释放魔法，豆子变成有着特定行动机制的怪物，然后去解开一道道谜题。它的机制在于一开始每个豆子就存在于一套系统内，后面是系统之间的回合制交互，学习曲线比较陡峭。难度很足。

→ 游戏获取

[Steam 上的 Bean and Nothingness](https://store.steampowered.com/app/1706090/Bean_and_Nothingness/)

---

# 映像

现实拟像放映——

![6d9c266fc4e3475fb12f94f50e2fa86c.jpeg](Scenes%20Weekly%20%2336.assets/6d9c266fc4e3475fb12f94f50e2fa86c.jpeg)

{上图：James Webb Space Telescope - Primary Mirror Segment Cryogenic Testing}

摄于2011年4月14日，工程师检查韦布望远镜18枚主镜片的前6片。

Image Credit: NASA/MSFC/David Higginbotham

---

喜欢本文的话，欢迎分享、订阅。

第 35 期请[在此查看](./Scenes Weekly #35.md)。

本次封面使用了 Brygada 1918  字体。