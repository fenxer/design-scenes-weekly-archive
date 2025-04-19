# Scenes Weekly #55

2022-05-23

\> 设计视角下的世界——

第 54 期请[在此查看](./Scenes Weekly #54.md)。

本期出现：

- 非生产力优先记录工具 mysc. 初见
- 对 Bionic Reading 提高阅读效率存疑
- 2022 年酒水包装设计展望
- 其他：iOS 创新辅助功能、Substack 的「友链」、What human foods can dogs eat、RGB Rush 小游戏

如有格式异常建议点击最上方「在浏览器中访问」。

---

# 杂事

1、在笔记应用层出不穷的今天，mysc. 作为一个非生产力优先的工具让我感兴趣。

> mysc. 是一个为生活而设计的记录工具，希望让更多普通人能够自由的记录，创作和发布。

—— V2EX [原帖](https://www.v2ex.com/t/852431)

![1669799503246.png](Scenes%20Weekly%20%2355.assets/1669799503246.png)

{上图：mysc. 首页和笔记的详情页}

在 mysc. 点击上方输入框便可记录内容，长按内容块可多选和批量操作，长按黑色竖线位置可拖拽合并和加入专集（加入后会在首页消失😳），横划可引用当前内容块发布新内容。横划的操作让人想到了 [Craft](https://www.craft.do/)，不同的是在 Craft 中横划一行内容即可选中并进行大多操作，mysc. 则区分开这些功能到三种交互形式。至于孰优孰劣，由于侧重点不同，看个人体验吧。

点进一个内容块，在详情页可以通过「想了又想」补充后续。是个不错的文案，可惜对比度太低了。提到界面设计这里，mysc. 给我的感觉有些「平面化」，是那种「自由的感觉」。像我这种不自由的人，可能就会把首页设计成这样——

![1669799504392.png](Scenes%20Weekly%20%2355.assets/1669799504392.png)

{上图：mysc. 首页重设计}

- 我更倾向于把输入框放在底部方便单手交互；
- [HIG 里](https://developer.apple.com/design/human-interface-guidelines/ios/bars/tab-bars/)虽然没有提到 Tab Bars 的数量建议，但是 2 个的话我倾向于将功能拆分并置于顶部；
- 界面中大量使用了 #000 纯黑字色，不太合适；
- 包括纯黑的竖线，我更倾向于淡化以突出内容，或者干脆用上 logo 中那一抹橙色；
- 上面提到首页的内容块加入专集后会在首页消失，目前还没找到返回首页的方法，让我有点不知所措。看来官方想把首页当成一个临时的专集，每条内容的归宿都是特定的专集。但是如果把首页当成一个总的合集时间线呢；
- 依照上一条，将来记录内容越来越多的话，我倒是想要个按照日期回溯的功能。虽然官方提到，在输入框撰写内容时，写到关键词会自动提示以往的卡片。所以日期筛选那里可能会是一个更轻量 & 优雅的方式去解决；如果不需要上一条的假设，那边也不需要日期的筛选。

注意，这仅是一个设计实验。产品还处在早期，还有更多可以选择的走向。希望他们做出一个更有趣的产品，而不是像我一样拘束在框架之中。

→ 官网

[mysc.](https://www.mysc.app/)

---

2、在 iMore 上看到了 Bionic Reading 的[新闻](https://www.imore.com/viral-bionic-reading-tool-iphone-and-mac-will-blow-your-mind)（or 广告？），这项技术貌似已存在数年，最近公布了 API（收费），到官网一看还申请了专利。Bionic Reading 的原理是，你在读一个单词或一句话的时候会先注视单词前半部分然后脑中自动补全后面。往下翻到示例文本，我直接地铁老人看手机——

![1669799505269.jpeg](Scenes%20Weekly%20%2355.assets/1669799505269.jpeg)

{上图：左边是一段字体偏细的正常文本，右边是经过 Bionic Reading 技术处理后的文本}

我的第一感觉是，这些看起来像是机械加粗的字体，不光打乱了原有的加粗强调功能，最严重的是扰乱了字体负空间（字体外形）导致更难以阅读。在[第 23 期](https://mp.weixin.qq.com/s/trmup73B9Qw2MNgBiLmLIg)有一篇文章介绍了易读性与行长的问题。其中分析了人眼扫视阅读时的状况：

![1669799506089.png](Scenes%20Weekly%20%2355.assets/1669799506089.png)

{上图：阅读时视线分析}

与 Bionic Reading 那[专利](https://data.inpi.fr/brevets/FR3052587)不同，Parker 等人研究提出，英文阅读习惯中，阅读到末尾回扫下一行开头时，视线焦点（即中央凹）并非准确落在第一个单词上，而是稍向右的一处地方，由余光（旁中心凹）来补完开头单词。在官方推荐的应用 Fiery Feeds 中，Bionic Reading 是这样应用的：

![1669799506927.png](Scenes%20Weekly%20%2355.assets/1669799506927.png)

{上图： Fiery Feeds 中启用 Bionic Reading 后的正文、相关设置与中文}

结果就是 Bionic Reading 的加粗打乱了我的阅读节奏，让中央凹强制落在了不恰当的地方，当用旁中心凹扫视旁边单词时，再次因加粗导致的负空间改变而扰乱识别。让人不得不仔细注视单词是什么。阅读得很累，调节几次 Fixation 和 Saccation 后依旧无果。中文更甭提，根本不适用。

不同人的阅读方式或许不同，我也不是英语母语者，Bionic Reading 对我来说基本是负体验，远没有新闻中提到的如何惊奇。顺便一提，官方之前把自己推销到 Show HN 上，最前面的回复批评他们没必要把申请专利的闭源 API 发到 HN 上……

那么 Bionic Reading 对你有帮助吗？

→ 官网

[BR for You.](https://bionic-reading.com/)

---

3、专注于酒水包装设计的 CODO Design 分享了对 2022 年行业的一些展望。文章先是分析了行业背景，比如波尔公司（Ball Corporation）将最低订单量从 1 提升到 5 货车荷载，这可能影响到 90% 的酒水厂商的包装选择，也间接影响到设计上对于材料的考究，加速了包装形式多样化。

激烈的市场竞争、推陈出新的售卖形式以及增长缓慢的销售，都使得客户重塑品牌的需求热度不减。专注品牌建设时，CODO 认为现在的趋势是找通过品牌调性准目标人群，而不是把凡是想喝酒的大众都定为目标——也就是 "lifestyle" 一些。比如都市白领喝 PBR（蓝带），玩滑板和重金属音乐的喝 Liquid Death 等，通过人群共性来反向决定品牌营销基石，最终反映到消费者自己对所在人群的定位。

![1669799507834.jpeg](Scenes%20Weekly%20%2355.assets/1669799507834.jpeg)

{上图：各个啤酒品牌营销材料图 1. Liquid Death, 2. 805 Beer, 3. YETI, 4. Dogfish Head x Merrell, 5. Montucky Cold Snacks, 6. Pabst Blue Ribbon}

渠道也是很重要的一环，在线商店的目的不光是卖货，重要的是收集掌握消费者数据，以进行后续的营销活动（这点哪里都一样呢）。除了传统的啤酒，还有很多像是硬苏打水、即饮（RTD）鸡尾酒、风味麦芽饮料（FMB）和无酒精饮料（NA）等赛道选择。甚至还要加上不同饮用时段（早中晚）对饮用需求也有所不同这一因素，都在影响着设计呈现形式。

![1669799508763.png](Scenes%20Weekly%20%2355.assets/1669799508763.png)

{上图：CODO 品牌架构示意}

如上图 CODO 的一个品牌架构示意，步骤大概是先为客户定下总的品牌概述，在针对不同生产线面对的人群，从定位触发一步步推导出品牌具象的一些设计标签。

最后第四节 CODO 终于谈到了具体的包装设计趋势。精酿啤酒的小众、独立自主的概念与华丽的定制插画不谋而合。但是哪里的设计都是莫比乌斯环，当大家都在趋同设计时就要周期性地拉开差异化。CODO 表示这些啤酒厂客户接受极简主义，但是作为包装要抢眼，还要再多一些「设计感」脱颖而出。

有些厂商则是走出现代设计的循环，径自寻找自己的复古经典。不过令我感到好奇的是，CODO 把单线条（Monoline）描边的方式归为「专为 DTC 打造的美学」。对于这些 Behance 的「常客」，也不过是环中的一个周期。

![1669799509714.jpeg](Scenes%20Weekly%20%2355.assets/1669799509714.jpeg)

{上图：一些 Monoline 风格的包装}

其他常见的元素还有头骨💀、异形包装、创意互动包装等。第五节是对从业人员以及分析师的一些采访，信息相当充实。

→ 详见原文

[2022 Craft Beer Branding and Package Design Trends - CODO Design](https://cododesign.com/2022-beer-branding-trends/)

---

4、iOS 的设置中，辅助功能有着最多的设置项。上周 Apple 在 Newsroom 展示了一些创新辅助功能——

- 放大器能为失明或低视力人士检测门扉，看起来像是 Apple 机器视觉技术的冰山一角；
- A11y 中有一项不成文的结论，即满足无障碍设计的同时，也会为普通用户带来便利或新体验。「Apple Watch Mirroring 可以帮助用户使用配对的 iPhone 远程控制 Apple Watch，从而让肢体或运动障碍人士能更加便捷地使用 Apple Watch。」同样如果有 Apple Watch 录屏需求时，也可以使用 AWM 来完成，而且从图中看起来，AW 显示屏幕也大了好多。然而只适用于 S6 以及后续机型；

![1669799510898.png](Scenes%20Weekly%20%2355.assets/1669799510898.png)

{上图：Apple Watch Mirroring 演示，Apple Watch 映射在底部弹出的 sheet 中}

- 实时字幕是早在 Pixel 系列上就有的功能，也是只支持英语；
- …

→ 其他功能详见原文

[Apple 展示创新辅助功能](https://www.apple.com.cn/newsroom/2022/05/apple-previews-innovative-accessibility-features/)

---

# 摘录

这周看过的一些——

> It amazes me that in the 8 years since Apple CarPlay and Android Auto were released, very few carmakers have built systems that can rival those running on our phones. In theory, carmakers can offer something much more valuable because Apple CarPlay and Android Auto hardly exchange any data with the car, making them quite simple. Yet, it is taking embarrassingly long for carmakers to figure it out and Porsche is not even close.

—— Casper Kessels - [Driving a Porsche Taycan for a Week, a UX review](https://www.theturnsignalblog.com/blog/taycan-roadtrip/)

---

# 小事

1、Elon Musk & Twitter 这场戏「不出意料」地没有顺利收官，spam 占 mDAU 多少可能只有 Twitter 还在关心，焦点在于科技股票持续下跌的背景下 54.20 还是否划算，以后背后不为人知的金融游戏。一出「纸牌屋」的戏码，Musk 似乎更想演成「是，首相」。还是看看正常信息吧——

![1669799511835.png](Scenes%20Weekly%20%2355.assets/1669799511835.png)

{上图：出自《爱，死亡和机器人》第三季第一集}

哦不对，不是这个——

距离 Substack 作者互相推荐功能上线已过去一个月，Substack 上周发文表示此举显著加速了各个 publication 的增长。举例中包括本通讯的「熟客」Lenny 's Letter 和 First1000。官方表示，当你推荐 1 位 publication 时，你可能会获得 3 倍的被推荐机会。[网络效应](https://designscenes.zhubai.love/posts/2117545871552929792#:~:text=%E7%B3%BB%E7%BB%9F%E6%8E%A8%E9%80%81%EF%BC%89%EF%BC%8C%E9%82%A3%E4%B9%88-,%E7%BD%91%E7%BB%9C%E6%95%88%E5%BA%94,-%EF%BC%88%E7%BD%91%E7%BB%9C%E5%A4%96%E9%83%A8%E6%80%A7)开始显现。

![1669799512992.png](Scenes%20Weekly%20%2355.assets/1669799512992.png)

{上图：Substack 管理推荐}

虽然我们早在几年前的公众号以及更早的博客友链中，就看到过类似机制，但 Substack 做进了产品里，作者能在后台看到我推荐了谁和谁推荐了我。在 publication 首页和关注后都能看到作者的推荐。

![1669799514079.png](Scenes%20Weekly%20%2355.assets/1669799514079.png)

{上图：关注作者后的推荐列表}

上图中，推荐的作者其实不止 4 位，但是没有滚动条等任何提示，在 Substack 关注后的流程中类似的优化点还有不少。另一方面又有些担忧推荐位的滥用🤔，消耗个人的信用。

→ 原文

[https://on.substack.com/p/recommendations-update](https://on.substack.com/p/recommendations-update)

---

2、Pawmenow 有个小工具可以查询什么食物人能吃狗不能吃。可以返回能吃、不能吃和有争议三种结果。

![1669799515024.png](Scenes%20Weekly%20%2355.assets/1669799515024.png)

{上图：查询三种食物后给出的结论详情}

有个问题是，查询后看不到详情在描述哪个食物。

→ What human foods can dogs eat

[What kind of human food can dogs eat safely? [Quick Answers]](https://www.pawmenow.com/what-dogs-can-eat/)

---

3、RGB Rush（中文名：色速）是一款以颜色为主题的游戏，给定一个颜色，你需要快速地拖动滑块来去合成尽可能贴近的颜色。虽然玩法很简单，但游戏的手绘风格很不错。

![1669799516311.jpeg](Scenes%20Weekly%20%2355.assets/1669799516311.jpeg)

{上图：HSV 关卡可能是最简单的}

→ 游戏获取

[Steam 上的 色速](https://store.steampowered.com/app/1952760/)

---

4、最近看了两周 Axios 的推送，感觉他们的 newsletter 写的真不错，简洁、清晰、高效——实际上这很难做到，我觉得比 [Morning Brew](https://www.morningbrew.com/daily) 更易读。在邮件的底部看到使用的是一项 Smart Brevity® 的技术，集成在他们专用的 Axios HQ 工具中。这虽然给我带来了一些启发，但实际还是有些难以写作…… 好处在于目标又多了一个。

![1669799517851.gif](Scenes%20Weekly%20%2355.assets/1669799517851.gif)

{上图：Smart Brevity® 的原理展示}

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周更新了 0 个。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

---

# 劳逸

![1669799519077.png](Scenes%20Weekly%20%2355.assets/1669799519077.png)

{上图：仁王 2 截图，主角抱着的巨大猫怪游戏中称为「善擦」}

上回书说道 Team Ninja 的最终幻想起源（FFO）以流畅战斗在系列中脱颖而出。这次在尝试了仁王 2 后感觉 FFO 更像一个减负后的仁王。同样不对剧情有所期待，仁王 2 的战斗系统深度和地图复杂度都强于 FFO，特别是前者的成功，打造起了不同于 FromSoftware 的 ARPG 标杆。遗憾的是堆怪与敌人重复度高，与一些攻击动作的不断「复读」，导致后面没什么太大动力——但从好友的评价和游戏时间来看，这些应该只是我个人偏好问题。

→ 游戏获取

[Steam 上的 Nioh 2 – The Complete Edition](https://store.steampowered.com/app/1325200/)

---

# 映像

现实拟像放映——

![1669799519989.jpeg](Scenes%20Weekly%20%2355.assets/1669799519989.jpeg)

{上图：青色台灯射下黄色的具象光线照在酸橙上}

© Priscilla Ong

---

# 温故

→ Scenes Weekly #6

[Scenes Weekly | No. 6](https://mp.weixin.qq.com/s/J95aVxVCvzvwHcGDDYsUiA)

- Google I/O 2021, Material You!
- Material Design 中的无障碍设计
- Android 12
- Google 数据安全改进
- 缝合了 Notion 和 Coda 的 Smart Canvas
- 垂直居左导航特点浅析
- Twitter 机器剪裁算法的弊端与调整

---

喜欢本文的话，欢迎分享、订阅。

第 54 期请[在此查看](./Scenes Weekly #54.md)。

本次封面使用了 Pramukh Rounded (Variable) 字体，灵感为 emoji 中的虚线脸🫥。