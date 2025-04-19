# Scenes Weekly #53

2022-05-09

设计视角下的世界——

第 52 期请[在此查看](./Scenes Weekly #52.md)。

本期出现：

- Occlusion Grotesque 木制实验字体
- DELIGOGO 便利店品牌风格鉴赏
- 12 轴可变字体 Roboto Flex
- Unicode 与文本工具
- WSJ 订阅体验批评
- 其他：Color Orbs Maker、Twitter Circle、Instagram、Fable Figma 插件、Microsoft 3D Movie Maker 开源、Airbnb CEO 总结、机械表原理、Brave Search 主管访谈

如有格式异常建议点击最上方「在浏览器中访问」。

---

# 杂事

1、Occlusion Grotesque 是一款…… 由森林里的树设计的实验字体。Bjørn Karmann 这个项目令人拍案叫绝，首先他在一棵树的树皮上刻下所有字母，然后每隔一年观察树皮愈合后字母的形状，如下图。

![1669796095546.jpeg](Scenes%20Weekly%20%2353.assets/1669796095546.jpeg)

{上图：小写字母 j 四年来在树上的发生的变化}

之后 Karmann 使用佳能 5D MKII 相机按照固定比例拍摄并临摹下所有字形，根据这些去制作字母的字重变化，就成了 Occlusion Grotesque 这款独特的生物字体。

![1669796097284.jpeg](Scenes%20Weekly%20%2353.assets/1669796097284.jpeg)

{上图：Occlusion Grotesque 所有字型}

再之后 Karmann 使用 GANN 以刚才的数据去训练一个 AI，可以展示出其他字母刻在树皮上 4 年后的变化，太酷了。

→ 项目详情以及字体获取

[Occlusion Grotesque - Bjørn Karmann](https://bjoernkarmann.dk/occlusion-grotesque)

---

2、北京青年路地铁站 D 口的 DELIGOGO 便利店去年一开业便广受欢迎，背后操刀设计的是 Meat Studio。这套连带汉字定制的像素化风格品牌，「很难想象出」客户为北京地铁。

![1669796099578.jpeg](Scenes%20Weekly%20%2353.assets/1669796099578.jpeg)

{上图：DELIGOGO 标识一览，图来自 Meat Studio 项目页}

Meat Studio 的设计理念是把便利店物品包装成复古游戏里的「掉落物品」，上 / 下班的打工人路过此处可以获得一些 buff，以迎接 / 送走一天快节奏又忙碌的生活。我们可以看到一些像素图形里的细节，比如有很多为了提升认识度而打破全像素设计常规的次像素（sub-pixel）：

![1669796102357.png](Scenes%20Weekly%20%2353.assets/1669796102357.png)

{上图：手提袋上的黄色像素星星}

一般像素 sprite 的色值矩阵都是一一对应的（例如 [Indexed color](https://en.wikipedia.org/wiki/Indexed_color) 技术），不会出现一个格子里两个颜色，当时的次像素问题一般产生于 sprites 运动后的速率（比如常一些 SFC 游戏穿墙捷径开发）。

![1669796104136.jpeg](Scenes%20Weekly%20%2353.assets/1669796104136.jpeg)

{上图：FF DOT 一书中最终幻想初代黑魔法师像素排列}

所以个人觉得，这套标识更多的还是黑白画布与精心挑选的颜色之间的撞色对比，次像素化让图形在复古和现代之间找到了平衡，配套定制的汉字也是点睛之笔。很喜欢，这阵疫情过去后有机会该去打个卡。

→ 项目详情

[gogo — Meat](https://meat.studio/gogo-1)

---

3、继 Roboto Slab、Roboto Mono 和 Roboto Serif 后，Google 为 Roboto 字族推出了目前为止最重磅的 Roboto Flex 可变字体。开局王炸，12 个可变轴体（意味着需要 12+1 个母版），其工作量就让几乎所有可变字体汗颜。其中还配备了 [Optical Size](https://fonts.google.com/knowledge/glossary/optical_size_axis) 这种微调轴。当年的 GT Flexa 也才 3 个轴。

![1669796107219.png](Scenes%20Weekly%20%2353.assets/1669796107219.png)

{上图：这也是 Roboto}

12 个轴为 Weight、Width、Slant、Grade 和 Optical Size 五个基础轴，以及 Ascender Height、Counter Width、Descender Depth、Figure Height、Lowercase Height、Thin Stroke、Uppercase Height 七个高级参数轴。关于这些可变轴的介绍，在[原文](https://material.io/blog/roboto-flex)中也有详细解释，相当于使用前的说明书。

→ 获取字体

[Google Fonts: Roboto Flex](https://fonts.google.com/specimen/Roboto+Flex)

---

4、Danny King 做了一个 Color Orbs 生成器，可以根据最多 5 种颜色、图案和 4 种参数生成千变万化的彩绘球体。可随机生成，支持保存生成的动态视频。使用的是 p5.js。

![1669796109008.png](Scenes%20Weekly%20%2353.assets/1669796109008.png)

{上图：King 的 Color Orbs Gallery}

→ 自己设计

[Danny King: Generative Art | Color Orbs - Designer](https://www.dannyking.uk/artwork/colororbs/designer)

---

5、THE ECLECTIC LIGHT COMPANY 分享了几个文本相关的实用工具。Nalaprop 可以帮你解析自然语言（分词、词频等），Apfelstrudel 可以显示输入文本的四种 Unicode Normalize 格式，包括 HFS+ 中的支持字符核对（HFS+ 中 以 UTF-16 格式并以 NFD 形式规范化），举个例子：

![1669796111014.png](Scenes%20Weekly%20%2353.assets/1669796111014.png)

{上图：在 Apfelstrudel 输入 å 作为示例}

这个 å 是我随便复制粘贴过来的，Apfelstrudel 告诉我们这个字母是单个 code point，因为按照规范分解完又会组合归一，这是 NFC。NFD 是规范分解后不组合，所以两者之间会有 1 长度的差异。复制绿框处建议的字符，便可在 HFS+ 系统中规范使用字符。

当然一般来说 macOS 会帮你自动转换，这个应用还是比较适用于文本分析或者命令行复制粘贴的场景。平时偶尔出现的 PDF 乱码也和 Unicode 这四种规范形式有关。Unicode 官方就有一篇很不错的 UNICODE NORMALIZATION FORMS [介绍](https://unicode.org/reports/tr15/)。

Dystextia 则是利用这个规则去生成混淆文本。另一边 Rosettavert 可以实现在文本的不同编码转换，这个需求正常多了。

→ 原文还有更多工具

[Text Utilities: Nalaprop, Dystextia and others](https://eclecticlight.co/text-utilities-nalaprop-dystextia-and-others/)

---

6、一些传统媒体的在线订阅体验远没有买报纸看体验流畅，我们都知道这些体验很烂，Built for Mars 就展现了 The Wall Street Journal（华尔街日报）的订阅流程是如何一步比一步泥泞不堪的。首先在文章页面，订阅选项元素堆叠没有重点，订阅套餐之间无法直观比较，最不能忍受的是密码位数有上限（15 位），订阅后便是一系列冗长的设置。从开始到订阅结束回到文章，高达离谱的 26 步：

![1669796112784.png](Scenes%20Weekly%20%2353.assets/1669796112784.png)

{上图：WSJ 订阅流程一览}

一番折腾后还无法回到最开始的新闻页…… 大多数人都会安慰自己，没事下一次点开文章就没有付费墙了。然后到退订的流程才发现真正的地狱刚开始——需要打电话人工退订，使用客服机器人都算友好的。

老样子，Peter 在文章下方总结了几个设计要点，相对于这些常见的负面用户体验 WSJ 明知故犯，本通讯的批评主义火花又被点燃了。

早在 2018 年加州法律就规定必须允许读者在线取消订阅，但是直到去年三月份， 美国大多新闻机构在退订方面依然我行我素（[报道 1](https://www.niemanlab.org/2021/03/most-u-s-news-organizations-still-wont-let-readers-cancel-their-subscriptions-online/)）。十月末，FTC 裁定这种行为是 “dark patterns that trick or trap consumers into subscriptions” 欺诈行为，如果读者是在线订阅，就必须可以在线取消订阅，且要易用。但正如你所见，纽约时报和华尔街日报等大型新闻媒体并没有搭理 FTC，FTC 也未对执行置评（[报道 2](https://www.niemanlab.org/2021/12/ftc-let-digital-subscribers-click-to-cancel-newspapers-hey-not-so-fast/)）。

→ 详见原文

[Why is the UX of paid journalism so bad? 🧠](https://builtformars.com/case-studies/wsj)

---

7、几个小更新：

7.1、网页动效设计工具 Fable 发布了 Figma 插件，无需账户，可以直接复制 Figma 图层到 Fable 中。当然一些高级样式会丢失。

→ 插件地址

[Figma](https://www.figma.com/community/plugin/1093136289410156578/Fable-Export)

---

7.2、Twitter 正在小范围内测 Circle 功能，最多可以让你给 150 人分享推文。Twitter 认为这比关注才能看的「受保护帐户」功能更灵活。然而群众只悼念 Google+，我还看到[有人在十年前](https://web.archive.org/web/20111105211217/http://www.geekybuddha.org/blog/2011/07/16/twitter-should-copy-google%E2%80%99s-circle-feature/)就提到过这事。Twitter 一直在重塑用户推文的矢量性，这是自社区功能的后又一相应举措。

→ About Twitter Circle

[About Twitter Circle](https://help.twitter.com/en/using-twitter/twitter-circle)

---

7.3、Instagram 正在测试一种全屏的（9:16 安全区）信息流首页。当效率不在是 feed 的首选——

![1669796114694.png](Scenes%20Weekly%20%2353.assets/1669796114694.png)

{上图：新信息流首页样式，顺便去掉了花哨的辣眼睛背景}

→ 听听 Adam Mosseri 怎么说

[登录 Twitter，关注Adam Mosseri](https://twitter.com/mosseri/status/1521589403671355392)

---

7.4、Google 据说正在测试桌面端 SERP 变为无限滚动。推测这会大幅度降低首页权重，但是有更多的广告展现机会。

→ 消息来源

[登录 Twitter，关注Brodie Clark](https://twitter.com/brodieseo/status/1521090389498757120)

---

7.5、Raycast for Teams 正处于 Beta 阶段，输入 0xC0C0A 即可解锁。Team 版允许团队内部在一个私有商店里开发、共享和发现扩展。

→ Guide

[Getting Started - Raycast API](https://developers.raycast.com/teams-beta/getting-started)

---

# 摘录

这周看过的一些——

> Look, Steve’s opinion specifically was at the beginning of the iPod project was, “We are going to make this amazing thing called the iPod” — we didn’t know it was called the iPod at that time — but “We’re going to make this thing, and this is going to drive Mac sales”. So to use the iPod, you’re going to have to buy a Mac, and that was his opinion.

> Two years in, the numbers were okay for the Mac fanboys who had Macs, but no one else was interested in switching to a Mac just for an iPod. So we had that data and it showed very clearly that that original opinion or that hypothesis was that more people would buy Macs because the iPod was available was not right. We had a few people, but it was not this huge mass of people switching from Windows to the Mac because the iPod existed and you had to have one. So over time, and this is the [third generation](https://commons.wikimedia.org/wiki/File:Ipod_backlight_transparent.png), we had to have the Windows connectivity, the Windows functionality, compatibility, to make sure it worked.

> And then all of a sudden people were like, “Oh, this iPod thing is really cool. I’m using it on my Windows device, on my Windows laptop, or what have you. But I wonder what the full Apple experience would be?” And then people started buying Macs after they got a taste of the Apple experience with the iPod on their Windows based computer.

—— Tony Fadell

---

# 小事

1、微软开源了 Microsoft 3D Movie Maker 代码，这款 1995 年的应用代码需要 Visual C++ 2.0 编译运行。我也趁机回顾了下，这款软件在打入日本市场时发布了多啦 A 梦的资源拓展包。而且早年的交互都非常有创意，比如下图打开其他媒体文件的动画：

![1669796116426.gif](Scenes%20Weekly%20%2353.assets/1669796116426.gif)

{上图：M3MM 中选择 Watch another movie}

顺便一提，Comic Sans 的初登场便是在 Microsoft 3D Movie Maker 中。而且至今依然有 [3DMM 社区](https://www.3dmm.com/)在活跃。那个年代的微软虽然也没啥审美，但是做出了不少像 Microsoft Comic Chat 之类的有趣产品，关于 MCC 写过一篇简单介绍的[文章](https://fenx.work/Microsoft-Comic-Chat-5e90635ad9ad4d06a613e94c553f4392)。

→ GitHub Repo

[GitHub - microsoft/Microsoft-3D-Movie-Maker: This is the source code for the original Microsoft 3D Movie Maker released in 1995. This is not supported software.](https://github.com/microsoft/Microsoft-3D-Movie-Maker)

---

2、Airbnb Q1 财报增长强势，营收 15.09 亿美元，同比增长 70%，税前利润 2.29 亿美元，实现首次 Q1 盈利。Brian Chesky（CEO）用 Twitter Threads 上进行了总结（财报电话会议后一天）：

- 精简业务，回归初心；
- 削减项目，忍痛裁员；
- 优化成本，严控固费；
- 灵活营销，重心公关；
- 重整品牌，适度支出；
- 静候良机，消费反弹；
- 久居用户，逐年增多；
- 功能迭代，百次有余；
- 更多分享，六日之后；

5 月 11 日，Chesky 将会继续分享 Airbnb 的十年历程。

![1669796118458.png](Scenes%20Weekly%20%2353.assets/1669796118458.png)

{上图：水彩风格插画配上 Travel is about to get a redesign，摘自 Airbnb Q1 股东信}

顺便一提，Airbnb 四月末宣布了[新的办公计划](https://news.airbnb.com/airbnbs-design-to-live-and-work-anywhere/)，在任何国家和地区、在家里或公司、甚至旅行办公，工资都不变。这就是 Airbnb 的员工 "redesign"。

→ 原推

[登录 Twitter，关注Brian Chesky](https://twitter.com/bchesky/status/1521582440783007745)

---

3、Bartosz Ciechanowski 可以深入浅出地，以可视化的方式去介绍各种事物背后的原理。而且他的可视化图形都是在 WebGL 里手动码出来的…… 太强了。上次介绍过 [GPS 原理](https://designscenes.zhubai.love/posts/2097250965601222656#:~:text=Bartosz%20Ciechanowski)，这次讲的是机械表原理。

![1669796120461.png](Scenes%20Weekly%20%2353.assets/1669796120461.png)

{上图：机械表中 Tick Tock 原理}

TikTok 的叫法来源于此处 Tick Tock。

→ 原文

[Mechanical Watch – Bartosz Ciechanowski](https://ciechanow.ski/mechanical-watch/)

---

4、[第 49 期](./Scenes Weekly #49.md)提到了 dkb 对于下一代互联网引擎的看法，这次他采访了 Brave Search 的主管 Josep M. Pujol ——

- 如今很多搜索引擎品牌只是利用了 Google 或 Bing API 去展示搜索结果。 独立搜索引擎开发复杂、成本高昂，Brave 深知难处，便通过收购 [Cliqz](https://0x65.dev/) 的方法建立自己的搜索引擎；
- 匿名构建索引的优化不容易，Brave Search 推出了 Web Discovery Project 项目让用户来帮助减少噪音与不相关内容。同时他们也有自己的人工评估团队，努力抵制一些镜像站的 SEO；
- 独立的搜索引擎将有助于把内容审核权利掌控到自己手中；
- Brave Search 92% 的内容是自己独立产生的，8% 借用于第三方搜索引擎去优化搜索结果。DuckDuckGo、You、Kagi、Neeva 等很多搜索引擎虽然也有类似机制，但是公开得不透明；

除此之外，原文还探讨了垂直搜索引擎、内容判断的立场、Goggles 等问题。最后主管也回答了什么引擎最适合你。

![1669796122865.png](Scenes%20Weekly%20%2353.assets/1669796122865.png)

{上图：搜索引擎选择图，自制}

→ 采访原文

[Interview with Brave Search | DKB](https://dkb.io/post/brave-search-interview)

---

5、几篇文章：

→ 介绍高尔夫一杆进洞保险（[链接](https://thehustle.co/the-strange-business-of-hole-in-one-insurance/)）

→ 枫言枫语播客第 67 期邀请了 V2EX 站长 [Livid](https://v2ex.com/member/Livid) 作为嘉宾闲谈。说起来和站长唯一的交集是加了 Steam 好友……（[链接](https://www.xiaoyuzhoufm.com/episode/626ba660bf39836fd02b78e9)）

→ 美国劳工统计局一份报告统计了 15 到 80 岁一生中，陪在身边的人所占用你清醒时间的百分比，Flowingdata 据此做了一个动态的图表（[链接](https://flowingdata.com/2022/04/22/changing-who-we-spend-time-with-as-we-get-older/)）

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周更新了 3 个。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

---

# 劳逸

![1669796125672.png](Scenes%20Weekly%20%2353.assets/1669796125672.png)

{上图：Peglin Banner}

哥布林弹球是一款融合柏青哥玩法的 Roguelike 游戏。

对比现实弹珠具有了很大的弹力，增加了不确定性。整体还是 Deck Build 那套玩法，需要组建不同的弹珠组合选择路线，打败关卡 Boss。遗憾的是整体除此之外就没有其他内容了（剧情也没有），且前中期难度略高，很容易产生挫败感。目前游戏处于 Early Access 阶段，依然有很多需要改进的内容，但核心玩法还是能给到一些惊喜的。

→ [游戏获取](https://store.steampowered.com/app/1296610/_Peglin/)

---

# 映像

现实拟像放映——

![1669796128058.jpeg](Scenes%20Weekly%20%2353.assets/1669796128058.jpeg)

{上图：白色毛绒上衣和灰色帽子在衣架上组成了北极熊🐻‍❄️身形}

Hang On! © Helga Stentzel

---

# 温故

→ Scenes Weekly#4

[Scenes Weekly | No. 4](https://mp.weixin.qq.com/s/5LnS8CWqGkTJRsfTMVE22Q)

- Clubhouse 糟糕体验
- Twitter Space 回顾
- Hoefler&Co. 的创始人 Jonathan Hoefler 分享喜欢的字型

---

喜欢本文的话，欢迎分享、订阅。

第 52 期请[在此查看](./Scenes Weekly #52.md)。

本次封面使用了 Roboto Flex 字体，灵感来自受精卵 2PN 结构，以纪念周日母亲节。

