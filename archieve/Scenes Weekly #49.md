# Scenes Weekly #49

2022-04-11

\> 设计视角下的世界——

第 48 期请[在此查看](./Scenes Weekly #48.md)。

本期出现：

- [Read.cv](http://Read.cv) Team Profile
- 下一代搜索引擎展望
- 数据可视化颜色指南
- Netflix 与广告的思考
- Cron 使用感受、Elon Musk in Twitter、Reddit r/Place、Morning Brew 一些数据、艺术市场报告 2022、Steam Deck 改进、网页 Mac 系统、RealityScan 扫描建模

如有格式异常建议点击最上方「在浏览器中访问」。

---

# 杂事

1、[Read.cv](http://Read.cv) 终于为企业招聘者做了主页 Team Profiles，它更适合小型团队。页面结构和普通用户不太一样，需要选择一些官方默认提供的问题去回答，以 storytelling 的思路去展现团队的风格。但当 “Team Pills”（团队的标签，官方叫法）这里，过多类型不一的标签反而降低了阅读效率。

![截屏2022-04-07 17.23.27.png](Scenes%20Weekly%20%2349.assets/%E6%88%AA%E5%B1%8F2022-04-07%2017.23.27.png)

{上图：官方提供的早期团队资料页}

另外也发现了一些「额外收获」，你能在这里看到各个团队的真实人员配置和工作流程是什么，没有业务之外的HR等人间隔传达，信息也更准确。比如 Figma 团队资料页面就介绍了他们的工作流，分享了对设计师与产品经理角色的理解：

![PM-Design.png](Scenes%20Weekly%20%2349.assets/PM-Design.png)

{上图：设计和产品的职业功能之间有很大的重合部分}

→ Introducing Team Profiles

[Introducing Team Profiles](https://read.cv/teams/about)

---

2、之前，独立博客引擎 [blogsurf.io](https://blogsurf.io/) 因独特的 MarketRank 反SEO算法（[详见](https://dkb.io/post/market-rank)）引起了不少讨论。后来作者 dkb 在他的博客上又写了一篇文章讨论下一代搜索引擎的模样。

Dkb 认为下一代互联网搜索引擎中，隐私的保护是必要的，但在引擎的定制上却有很多空间而不单单是现如今的查询语句。所以他认为 DuckDuckGo 的单一生意不长久（毕竟 DDG 不是非营利性组织），并列举了有着很多筛选器的 [Kagi](https://kagi.com/)，可搜索自己文档的内联引擎以及诸多优化的 [Neeva](https://neeva.com/)，以及SERP按网站为对象划分的 [You.com](http://You.com)（也是唯一不在 beta 测试中的）。还有对话视图的搜索 Andi，和完全独立算法的 Brave Search，Brave 虽然没有做太多展示优化，但是可社区化的定制引擎 Goggles（尚未上线）让它独树一帜。

毕竟科技发展的浪潮里，搜索引擎一直在被看做为流量门户，自身的创新作为一潭死水很长时间了。

→ The Next Google

[The Next Google | DKB](https://dkb.io/post/the-next-google)

---

3、Lisa Charlotte Muth 的这篇数据可视化颜色指南，可以事无巨细地帮你从零建立一套高度完整的、无障碍的颜色系统。Lisa 以现在的几家媒体风格为切入点，举例了总体风格走向，给出了大量颜色建议（比如性别、政党以及喜怒冷暖等概念），强调了颜色系统与品牌的联系——一个老读者是可以根据图表配色就能分清出自哪家媒体。

![截屏2022-04-09 17.15.41.png](Scenes%20Weekly%20%2349.assets/%E6%88%AA%E5%B1%8F2022-04-09%2017.15.41.png)

{上图：一些情感色彩联想，出自论文 Affective Color in Visualization}

原文还有大量的拓展信息，是一篇信息量相当丰富的文章。

→ A detailed guide to colors in data vis style guides

[A detailed guide to colors in data vis style guides - Datawrapper Blog](https://blog.datawrapper.de/colors-for-data-vis-style-guides/#fewer-hues-more-shades)

---

4、用了一周 Cron 日历，几个感受：

- 目前完全依托于 Google 日历，虽然也可以订阅自己 iCloud 日历，但还是单一了一些。
- 我有很多非工作之外的日程提示，但 Cron 目前无法区分工作与非工作的场景，没有分组显示的开关（只能单个开关）；
- 界面很精致，比起其他日历应用乱乱的感觉要少一点。但更希望在「周」视图里更强调一下当日，之后日期强调的程度可以依次下降（未来的事不能说不重要，但也要先处理当前的事）。

目前 Cron 处于早期阶段，官方也在帮助页面上开了一个反馈需求的入口。期待越做越好。

→ 官网

[Cron | Early access](https://cron.com/)

---

# 摘录

这周看过的一些——

> A complex system that works is invariably found to have evolved from a simple system that worked. A complex system designed from scratch never works and cannot be patched up to make it work. You have to start over with a working simple system.

—— John Gall - Systemantics: How Systems Really Work and How They Fail

---

# 小事

1、在 Netflix 订阅增长放缓这个问题上，股东和分析师一直催促手握大量订阅用户的 Netflix 加入广告业务。之前的 Netflix 通过提升订阅价格来增加营收，但不同地区 ARPU 的差异让此项决策更容易陷进恶性循环——越涨价用户订阅增速越少财报不好看就越要涨价。Netflix 掩盖的理由是自家内容逐年增多，「账户价值」也随之增加，更不用说还加入了游戏等新型内容。但是对老订阅用户而言，包括游戏在内的媒体每消费过一次，其内容价值便指数性衰减一次，只有新内容值得维持订阅。这一基本盘又促使了 Netflix 源源不断的内容支出。

![netflix-1.png](Scenes%20Weekly%20%2349.assets/netflix-1.png)

{上图：Neflix 内部的增长焦虑，致使今年一季度增长预测仅为250万}

Netflix 的原创独占内容是天然的注意力磁铁，广告业务则是将此部分观众注意力售卖给广告商。推出更低的付费订阅门槛，用广告弥补 ARPU，挽回即将流失的边缘用户和进一步扩大南美和亚太地区用户规模。再加上其他流媒体竞对像「Disney 全家桶」（Hulu、Disney+、ESPN+）已有前车之鉴，面对质问 Netflix 也只能哑口无言——

Netflix 原本的立场对广告非常强硬，读过 Netflix TechBlog 的人都能感受到他们对用户体验的在意程度，这可能也是他们不断涨价的自信之一。广告使整个界面低效，他们必须像处理视频封面一样慎重处理广告视觉和位置显示。广告还会打断正常观众的观看流程，最重要的是，用户的付费心态可能会改变——由为内容付费变成为减广告付费。

付费与广告变为负相关，这正是国内视频平台走过来的一条泥泞不堪之路。在消费者看来，付了钱还要继续看广告就像买断制游戏还有课金一样令人鄙夷。但实际上海外用户心态如何，还真不好说。毕竟……SheIn 和 Shopee 的成功也说明了一些事情。

![截屏2022-04-10 15.41.53.png](Scenes%20Weekly%20%2349.assets/%E6%88%AA%E5%B1%8F2022-04-10%2015.41.53.png)

{上图：Hulu 的订阅价格，带广告是每月6.99美元，无广告订阅是每月12.99美元}

——这对一家25年的公司而言，是一个关键的转折点。在 Ben Thompson [这篇文章](https://stratechery.com/2022/why-netflix-should-not-sell-ads-elon-musk-and-twitter/)里有位读者提出，Netflix 旗下大量独占内容，也可以作为可调用资产售卖给像 Roku、Pluto 甚至 YouTube 等有成熟广告业务的媒体。就像上面说的新内容值得维持订阅道理一样。这样 Netflix 也可以继续专注新内容创（shao）作（qian），同理，Netflix 对与其 IP 的运作也没有压榨至尽，也是一种保守（褒义）。

这一模式可以在 Sony——或者说 SIE——对待独占游戏的举措中得到些参考。之前独占 PlayStation 平台的 God of War (IV) 和 Horizon: Zero Dawn 都在 Steam 上取得了不错的销量，引得 Epic Game Store 直接购买下了 Final Fantasy VII Remake 的 PC 限时独占权。负面影响则是，让玩家一直揶揄的 “Only on PlayStation” 也进一步沦为笑谈——“Only on Netflix”也可能如此。

综上，你能看到资本基本是和用户体验挂不上钩的，立场不同而很难兼顾鱼与熊掌。为什么 PLG 模式背后的驱动点在业务人员来看是那么「普通而义务」，却只在近几年受到关注？叹息。

最后，在诸多因素之下，Netflix 会走向何方呢？

---

2、Elon Musk 加入 Twitter 董事会可以看做是上次 Jack Dorsey 卸任 Twitter CEO 的后日谈。加上 Parag Agrawal 这在去中心化上情投意合的三个人像是在对 Elliott Management 等投资者的权力抵抗。这个新闻仿佛有很多可以说的但又仿佛没有什么说的。Meme、股票、编辑按钮、言论自由，戏剧依旧在上演。

→ Elon Musk joins the Twitter board

[Elon Musk joins the Twitter board](https://www.platformer.news/p/elon-musk-joins-the-twitter-board)

---

3、Reddit 的 r/Place 活动大获成功，这家更喜欢大规模用户互动而不是愚人节meme 的公司在今年复刻了2017年的 Place 活动，这次活动更有组织性，除了亚文化当道外，也充满了民族主义与政治性，特别是一些 Twitch 主播对粉丝的号召。r/Place 娱乐的同时也在提醒我们，强势一方的煽动者们号召其跟随群体压制弱势群体这一点，哪里都存在。

顺便，Reddit 的一篇过往文章中介绍了 r/Place 的后端容量需求，他们预估的 333 updates/s 如今有 694 次之多。

→ How We Built r/Place

[How We Built r/Place - Upvoted](https://www.redditinc.com/blog/how-we-built-rplace/)

---

4、CNBC 对 Morning Brew 的一篇报道：

- Morning Brew 从300万订阅人数涨到400万只用了八个月；
- 2021年收入5000万美元，是2020年的2倍数还多。几乎都来自广告，利润率两位数（起码营销那里做的挺足的，很多 newsletter 都有他们的赞助）；
- CNBC 觉得时事通讯的订阅是有上限的，Daily Skimm 700万订阅后开始放缓；
- Morning Brew 的订阅者平均年龄是 30 岁，受众为 25-40 岁人群。
- Morning Brew 想通过并购进入更多垂直行业的媒体中；

→ 原报道

[Morning Brew tops 4 million newsletter subscribers as it looks to expand with M&A](https://www.cnbc.com/2022/03/28/morning-brew-tops-4-million-subscribers-as-it-looks-to-expand-with-ma.html)

---

5、Art Basel 和 UBS 联合出品了 The Art Market 2022 报告。报告表示 2021 高端艺术收藏领域增长强劲，带动了整个行业复苏，但加剧了行业的头重脚轻，七成收藏家依然对市场抱有乐观状态。

当然 NFTs 已是无法脱离艺术市场的话题。报告里除了实在的数据之外，剩下的基本都是老生常谈。

→ 获取巴塞尔艺术展与瑞银集团环球艺术市场报告

[Download for free: The Art Market](https://artbasel.com/about/initiatives/the-art-market?lang=zh_CN)

---

6、第45期提到了 Steam Deck 早期系统的诟病，之后 Valve 就一直不断在听取社区反馈，积极改善这些问题。比如任天堂「做了五年」的收藏夹也一起更新了。看[演示视频](https://www.youtube.com/watch?v=x17p_wqPPc4)已经流畅了不少，

![截屏2022-04-09 20.53.37.png](Scenes%20Weekly%20%2349.assets/%E6%88%AA%E5%B1%8F2022-04-09%2020.53.37.png)

{上图：可以调节 TDP 和显卡频率的功耗选项}

[Build in Public](https://designscenes.zhubai.love/posts/2109939895006105600) 这里 V 社自推出[实验室](https://store.steampowered.com/labs/)系列功能以来就很出色，以至于每次都像精神股东一样分享出来。但作为设计人员的一面，又只能感叹他们设计债过于沉重，到现在还能看到青睐之光时期的一些设计元素混用。

→ Steam Deck 满月啦

[Steam Deck - Steam Deck 满月啦 - Steam 新闻](https://store.steampowered.com/news/app/1675200/view/3220644827954565733)

---

7、Infinite Mac 是一个基于浏览器的 Mac 模拟器。有 Mac OS 8.1 和 System 7.5 两个版本可以体验。

![截屏2022-04-09 18.38.16.png](Scenes%20Weekly%20%2349.assets/%E6%88%AA%E5%B1%8F2022-04-09%2018.38.16.png)

{上图：网页中运行的Mac OS 8.1}

→ 8.1

[Infinite Mac](https://macos8.app/)

→ 7.5

[Infinite Mac](https://system7.app/)

---

8、3D 扫描成像中，以往像 Capture、telegie（[第44期](https://designscenes.zhubai.love/posts/2109939895006105600)）等都要激光雷达摄像头进行深度定位。但 Capturing Reality 发布的 RealityScan 应用可以通过数十张图像来合成3D模型。但对相机的像素精细度、光线、背景和角度等因素有「不那么日常的」要求。[这篇新闻](https://www.theverge.com/2022/4/4/23010382/epic-games-realityscan-app-3d-models-smartphone-photos)能看到 The Verge 编辑的卖家秀体验。

→ Introducing RealityScan

[Introducing RealityScan: Now in Limited Beta](https://www.capturingreality.com/introducing-realityscan)

---

9、Ahmad 写了一篇文章去对比浏览器直接 Code 和用 Figma 做布局设计的区别。老实说开头没看懂他在讲什么……后面提了下各有优劣，但然后呢？可能这篇文章更适合前端开发看。

→ Tweaking In The Browser

[Tweaking In The Browser - Ahmad Shadeed](https://ishadeed.com/article/tweaking-in-the-browser/)

---

# 劳逸

![f778786a0b764b4daab684e883c25a57.png](Scenes%20Weekly%20%2349.assets/f778786a0b764b4daab684e883c25a57.png)

{上图：Patrick's Parabox}

推箱子永不过时！

比起 [Recursed](https://store.steampowered.com/app/497780/Recursed/) 的平台式解谜，Patrick's Parabox 更纯粹，递归效果更可视化，它不基于 Baba is You 式的语义规则，它就是推箱子，加入了递归要素去复杂化传统推箱子中位置逻辑规则。这是一部难得的关注已久却又没失望的游戏。

→ 游戏获取

[Steam 上的 Patrick's Parabox](https://store.steampowered.com/app/1260520/Patricks_Parabox/)

---

# 映像

现实拟像放映——

![444cbc0521b74786bd38d7e262e81a6f.jpeg](Scenes%20Weekly%20%2349.assets/444cbc0521b74786bd38d7e262e81a6f.jpeg)

{上图：1973年的互联网}

1973 年美国几所大学和企业组成的 ARPA 网络。

→ 出处

[登录 Twitter，关注David Newbury](https://twitter.com/workergnome/status/807704855276122114)

---

喜欢本文的话，欢迎分享、订阅。

第 48 期请[在此查看](./Scenes Weekly #48.md)。

本次封面使用了 Work Sans 字体，圆环样式灵感来自 WWDC 2022。