# Scenes Weekly #50

2022-04-18

\> 设计视角下的世界——

第 49 期请[在此查看](./Scenes Weekly #49.md)。

本期出现：

- 笔记与浏览器—— Beam 浏览器开箱体验
- 久等十余年的 Proxima Sera
- DALL.E 2 风险报告
- Elon Musk & Twitter | Season 2
- Spotify 假艺人依然活跃
- a16z The Marketplace 100 发布
- Httpie 如何失去 GitHub 54k stars
- Atlassian 宕机事故时间线整理
- 其他：DuckDuckGo for Mac、TikTok 的艺术市场、Mac App Store 欺诈应用、Playdate 掌机开屏动画、可随机文章的 Scrubstack

如有格式异常建议点击最上方「在浏览器中访问」。

---

暂停实验室上线了一个情绪急救的公益工具包。

> 如果你身处情绪风暴中，这个工具箱能快速给情绪降温，去做手头最重要的事情。……就像拥有了一个降落伞，即使身处困境，依然可以安全平稳降落。

→ 打开这个降落伞

[https://ebp.gesedna.com/pa-emotion-toolbox](https://ebp.gesedna.com/pa-emotion-toolbox)

---

# 杂事

1、[第47期](./Scenes Weekly #47.md)中提到的 Beam 浏览器，上周收到了 beta 邀请邮件。立马开箱试用一下，果不其然是 "WebKit + `Logseq`"（只是不想提 Roam，但其实 Beam 有 Roam 导入功能）。

![Beam - 1.png](Scenes%20Weekly%20%2350.assets/Beam%20-%201.png)

{上图：Beam on-boarding}

Beam 的新用户流程只有两步，一页登录另一页导入数据，均可跳过。只有在使用账户同步和发布内容时才需要登录账号。

![Beam - 2.png](Scenes%20Weekly%20%2350.assets/Beam%20-%202.png)

{上图：第三方工具识别 Beam 为 15.1 版本的 Safari}

Beam 的特色在于合并了笔记应用与浏览器信息源之间的路径。如上图，你可以直接按住 Option 键选择网页中的某块内容，点击一下就可以选择加入哪篇笔记，并且自动抓取了网页标题和链接。

![Beam - 3.png](Scenes%20Weekly%20%2350.assets/Beam%20-%203.png)

{上图：Beam 的几个截图}

做为浏览器的 Beam，目前自带了密码和去广告等隐私管理，无法安装任何插件。右键几乎没有人任何功能，只有刷新和检查元素。地址栏默认显示标题不显示网址让人觉得没有安全感。网页性能没碰到问题。

作为笔记应用的 Beam，以 daily notes 为主，支持双链和一些基本的语法，并且所见即所得，直接通过 Beam 官方服务发布内容。你可以把数据库备份到本地，也可以使用密钥在线同步。我觉得 Beam 团队对隐私的注重性比较靠近 DuckDuckGo——非必要不使用你的私人信息，同时也将卡片笔记做的门槛更低。

Beam 的核心开发团队来自 Apple，他们的设计也有十余年的工作经验。这是一款现阶段就足以令人期待的产品。

→ 官网

[Meet the bright web – beam](https://beamapp.co/)

---

2、本月 5 日，Mark Simonson 发布了 Proxima Sera 字体，距离知名的 Proxima Nova 发布已有 17 年……两者有着极为相似的高 x-height。

![Pro.png](Scenes%20Weekly%20%2350.assets/Pro.png)

{上图：上方 Proxima Sera，下方 Proxima Nova}

可以看到 subtle 那里上方有着相似的空间节奏，但是单个字母拿出来还有些不适应。比如下方的 a 和 e。

![pro - 2@2x.png](Scenes%20Weekly%20%2350.assets/pro%20-%202@2x.png)

{上图：Proxima Sera 与 Proxima Nova 的小写字母 a 和 e 对比}

小写 a 的字碗（bowl）连接处（connection）有着不同的风格，小写 e 的收尾虽然位置相同，但是不同的笔划粗细没有补正，反倒让 Sera 失去了 Nova 的一些辨识度——不太懂字体的我一眼也只能看到这些程度。

→ Proxima Sera

[Proxima Sera - Mark Simonson](https://www.marksimonson.com/fonts/view/proxima-sera)

---

# 摘录

这周看过的一些——

> Still I imagine that Twitter's bankers at Goldman Sachs will sit down with Musk's bankers at Morgan Stanley and Goldman will say “so uh where's the financing coming from” and Morgan Stanley will say “oh the financing is in this can” and hand Goldman a can and Goldman will open the can and a bunch of fake snakes will pop out. “AAAHHH,” Goldman will scream, and then they will chuckle and say “oh Elon, you got us again” and everyone will have a good laugh. Because, again, uniquely among public-company CEOs, Elon Musk has in the past pretended he was going to take a public company private with pretend financing! I am not saying that he’s joking now; I am just saying he’s the only person who has ever made this particular joke in the past.

—— Matt Levine - [Sure Elon Musk Might Buy Twitter](https://www.bloomberg.com/opinion/articles/2022-04-15/sure-elon-musk-might-buy-twitter)

---

## 小事

1、上周 OpenAI 的 DALL.E 2 爆火后，陆续有人收到测试资格，并在自己的博客和 SNS 上发布了更多了图片，我们可以借此一览 DALL.E 2 的强大。对艺术流派、镜头参数、时代等元素的模拟，对图像自身的解构，AI 的视觉表达迎来前所未有的飞跃。

客套话结束，细看 Twitter [#dalle](https://twitter.com/hashtag/dalle) 标签下的各种生成作品，最大的感受是 DALL.E 2 对模糊文案的解读，一组没头没尾的抽象词汇通过语法组合后就能得到「硅谷人偏好风格」的作品。生成的图像不能说笔触完全遵从现实逻辑，但也可以说其自身的美学具有高度的连贯性。谈论 DALL.E 2 以及之后的 AI 能否产生后现代主义之后的艺术运动有点不讨好，至少可以幻想一下，某一天我们是否会参观 AI 生成的艺术展。

还有很重要的一点是 DALL.E 2 的能力所带来的风险，OpenAI 的官方已经写了一份其潜在风险的[初步报告](https://github.com/openai/dalle-2-preview/blob/main/system-card.md)。报告中可以看到团队在去暴力去成人内容化等有害内容上做了很多努力，比如屏蔽了一些特定的词语组合（*像是「女人」和「洗澡」*），对人类黑话的去歧义（*像是区分茄子是蔬菜还是性暗示*），引入人性的偏见修正（*像是一提到 builder 就是白人男性*）等等。之前 Twitter 自动裁剪算法也出现过[类似的问题](https://weibo.com/6728914621/KgwSNglpI)。

→ 参考

[DALL·E 2](https://openai.com/dall-e-2/)

[A Few Things To Try With DALL·E](https://www.bramadams.dev/projects/dalle-tricks)

[Playing with DALL·E 2 - LessWrong](https://www.lesswrong.com/posts/r99tazGiLgzqFX7ka/playing-with-dall-e-2)

[登录 Twitter，关注Nick](https://twitter.com/nickcammarata/status/1511861061988892675)

---

2、同样也是[上期](https://designscenes.zhubai.love/posts/2125143039055626240#:~:text=%E8%B5%B0%E5%90%91%E4%BD%95%E6%96%B9%E5%91%A2%EF%BC%9F-,2,-%E3%80%81Elon%20Musk%20%E5%8A%A0%E5%85%A5)提到 Elon Musk 和 Twitter 的事情，但就在 11 号上期发布后不到一天，Twitter CEO Parag 说 [Musk 决定不加入董事会](https://twitter.com/paraga/status/1513354622466867201)，各种词汇意味深长，有人分析称可能为了不触发 Twitter 董事的 14.9% 股权限制，Musk 要有更多动作。14 号便以每股 $54.2 提出[收购要约](https://www.sec.gov/Archives/edgar/data/1418091/000110465922045641/tm2212748d1_sc13da.htm#ex-b_001)，这其实比去年十月份的每股 $60 左右要低的，所以中东股神的反对也是合情合理，他或许也在等待 Twitter 摆上私有化的拍卖台上。

这里面的分析已有太多文章，无法浓缩，可详见：

→ Sure Elon Musk Might Buy Twitter

[Bloomberg - Are you a robot?](https://www.bloomberg.com/opinion/articles/2022-04-15/sure-elon-musk-might-buy-twitter)

最可怜的是 Twitter 员工（甚至包括现任 CEO Parag），公司最近就像柳絮一样飘荡起伏，看不清未来的方向。虎嗅的一篇[公众号文章](https://mp.weixin.qq.com/s/dA7oRlnOIyTuBrYgyBMlFQ)称 Twitter 未来剑指 web3，但 Musk 其实[对这方面](https://twitter.com/yishan/status/1514939894719672326)并不敏感和超前，我更愿意相信他和 Jack 心中的去中心化是去利益后的 web3 协议，这是关乎 Twitter 的实体与概念性问题，所以我这种圈外人看 [SBF 的言论](https://twitter.com/SBF_FTX/status/1514588820641128452)就感觉有些疯言疯语。但不变的是就像赵长鹏投资福布斯一样，精英主义下的自由言论大概率是为自己的发言争取有利地位，马斯克已经是推特这个 playground 的得势者。平民主义下的自由言论则充满着危机，on 不 on chain 可解决不了道德哲学的难题。

→ 拓展：Twitter 开放算法遐想，这是 Jack 在职 CEO 期间最想做的事之一

[Elon is Right: Twitter Should Open Up the Algorithm](https://every.to/divinations/elon-is-right-twitter-should-open-up-the-algorithm)

---

3、作为「完美诠释『卖点广告怎么了』」的产品，DuckDuckGo 打算推出 DuckDuckGo for Mac 本地浏览器。采用了对 macOS 友好的 WebKit，重头构建，确保连第一方 cookies 也不会获取到你的信息，以及内置更多安全和隐私功能。自己造了一个标杆后，不知道 DDG 之后有没有兴趣做 "privacy benchmark" 服务。

不得不提的是，DDG for Mac 的测试资格获取很有意思。它的命题貌似是，如何获取尽量少而脱敏的用户信息去完成测试资格的发放。

![DDG.png](Scenes%20Weekly%20%2350.assets/DDG.png)

{上图：DDG for Mac 测试注册流程}

相比留下邮箱，DDG 只是把你提交的时间戳加入队列。或许这也侧面映现了那句隐私与便利性的「名言」。

→ 原文

[Introducing DuckDuckGo for Mac: A Private, Fast, and Secure Browsing App](https://spreadprivacy.com/introducing-duckduckgo-for-mac/)

---

4、Instagram 能吸引一大批艺术家的原因在于，它已是艺术市场渠道重要的一部分，很多策展人、艺术经销商和收藏家在上面「闲逛」。在上一期提到的[艺术市场报告](https://designscenes.zhubai.love/posts/2125143039055626240#:~:text=%E2%86%92%20%E5%8E%9F%E6%8A%A5%E9%81%93-,5,-%E3%80%81Art%20Basel%20%E5%92%8C)中，我们也能看到 Instagram 的重要性。

![截屏2022-04-16 18.04.34.png](Scenes%20Weekly%20%2350.assets/%E6%88%AA%E5%B1%8F2022-04-16%2018.04.34.png)

{上图：2021年高净值收藏家购买艺术品渠道柱状图，其中 ins 占有 31% 比例}

如今谈到社交媒体总是避不开 TikTok，Emilie 这篇文章探讨了 TikTok 上艺术家的现状，通过算法吸引而来大量受众，建立社群文化，增加销量，过上好日子。如果说 ins 是一个精心策展的在线画廊，TikTok 随手拍下的视频则多了几分生活色彩的真实。原来在两个平台就会处于两种语境的 artist 一词，更有希望通过 TikTok 打通这个隔阂。同样，走向极端也会派生出「绞尽脑汁 show 在明面上」，而忽视对艺术本身的思考。

→ TikTok: Art market disruptor or passing fad?

[TikTok: Art market disruptor or passing fad?](https://www.creativeboom.com/features/tiktok-art-market-disruptor-or-passing-fad/)

---

5、Spotify 上 "Fake Artist" 问题积弊已久。早在 2016 年 8 月，Music Business Worldwide（后简称 MBW）就[报道过](https://www.musicbusinessworldwide.com/spotify-is-creating-its-own-recordings-and-putting-them-on-playlists/)这个现象，国内你也能找到[相关报道](https://www.jiemian.com/article/1499223.html)。所谓的假艺人即指 Spotify 上一些靠玩弄推荐算法而播放量奇高的单曲背后署名，Spotify 官方层曾否认了这个灰色地带的存在。这些假艺人大多是瑞典人——瑞典也是 Spotify 的总部所在地🤔。

今年三月份，MBW再次报道了假艺人产业。Firefly Entertainment 公司靠这个获取了 700 万美元的年收入。经常出现在歌单 "mood and chillout" 里，最成功的「假艺人」之一 Christer Sandelin 单飞创建了 [Chillmi](https://chillmi.com/about/)，里面都是一些虚拟人物，靠这 2500 多首单曲年收入可达 54-170 万美元……瑞典当地报纸 Svenska Dagbladet 称 Spotify 在 2015 年曾直接委托他做一些适合 chillout  歌单的音频。

后来有 MBW 的匿名消息灵通人士给他们发邮件，叙述了一些行业内幕：比如 Alexa 和 Spotify 在内的大多数内容由数字流媒体平台（DSP）控制分发，用户大部分听歌场景都是点开歌单聆听 DSP 预先准备好的内容，一个愿打一个愿挨；做假艺人这种事索尼和环球音乐也在干等等等。

这些「假艺人」的背后虽然也是真人，但对于一个平台来说劣币驱逐良币的结果……很多读者对 Spotify 应该比我更熟悉，应该不用多说什么，更多信息请自行查看引用的链接。

→ 匿名信

[An MBW reader just blew open the Spotify fake artists story. Here’s what they have to say. - Music Business Worldwide](https://www.musicbusinessworldwide.com/an-mbw-reader-just-blew-open-the-spotify-fake-artists-story-heres-what-they-have-to-say/)

---

6、自从上次[IINA 事件](https://www.v2ex.com/t/658387)，我对 Mac App Store 的好感基本降到负数。MAS 常年审核随意与反馈缓慢，且一直没有改善。最近 Jeff Johnson 发推称某开发者仿照 Google 官方应用的几款产品上升到了免费榜靠前的位置（美区40名左右）。

![FQGlajnXIAEaZ9i.jpeg](Scenes%20Weekly%20%2350.assets/FQGlajnXIAEaZ9i.jpeg)

{上图：该开发者的一些应用}

这些应用都在标题上伪装成官方应用，并且免费下载。一旦进去就会先要求付费，很多冲浪新人就中招了。留下的一星评论也被官方刷的五星评论覆盖，导致分数还是 4.X 分。诚然这首先是开发者道德问题，但是一想到 Apple 每年吹嘘的 App Store 有多么多么华丽的数据，就不禁对那光鲜的背后产生烦躁。

→ Twitter Threads

[登录 Twitter，关注Jeff Johnson](https://twitter.com/lapcatsoftware/status/1513672378236166149)

---

7、Playdate 掌机刚推出时我一直不太看好，恰 old school 饭、没有肩键、像 NDS 一样反人体工程学、加个摇把当噱头、找来一群独立开发者例行营销生态……但最近看到 Easy Allies 的开箱视频有些惊叹，这个小东西的开机动画做的也忒好了。后续实机游玩估计第二阶段评测才能解禁。

→ Playdate Unboxing

[Playdate Unboxing and Hardware Impressions!](https://www.youtube.com/watch?v=ewPxuAFyY0c)

---

8、a16z 发布了 The Marketplace 100 - 2022（统计的是去年），前几年他们一直基于 GMV 统计这些私人交易平台（意外的简单粗暴…），今年加入了 MAU 和流量因素。疫情的反复催生了票务、餐饮、直播购物等民生娱乐类别的发展，虽然大部分在国内不做投资的话大都不了解。

![M100-Full-List 大.png](Scenes%20Weekly%20%2350.assets/M100-Full-List%20%E5%A4%A7.png)

{上图：The Marketplace 100 完整排行}

Valve 这次升到第二名，仅次于霸榜的榜一大哥 Instacart。充足的现金保证了他们的独立自主，否则可能也不会有 Steam Deck 产品了（？）Epic Game Store 一上来就排到了 20 名，撒钱还真有效果。相对比设计师的老熟人 envato 和 Toptal 就一直不温不火。

→ 详见原文更多分析

[The Marketplace 100: 2022](https://future.a16z.com/marketplace-100/)

---

9、悲报：Httpie 失去了GitHub 5 万 4 千颗星星，CEO Jakub Roztočil 亲自讲述了这一惨案。原本是像隐藏另一个 organizations 页面的 readme 文件，由于机构和个人页面有些相似，Jakub 现在自己个人页面 jakubroztocil/jakubroztocil 进行私有化操作之后，一个惯性在机构页面也「顺手」把 httpie/httpie 变为私有仓库，五万四千颗星星瞬间消失殆尽，而他应该操作的是 httpie/.github 那个仓库。

![confirm-B3X7QRNG 大.png](Scenes%20Weekly%20%2350.assets/confirm-B3X7QRNG%20%E5%A4%A7.png)

{上图：在 GitHub 进行危险操作时的确认弹窗}

GitHub 使用了统一的长段提示文案，并没有针对 repo 具体数据进行说明。如果一边提示「你将会丢失 54k stars」，另一边提示「你将会丢失 0 star」，那么警示效果会更好一些，通用的文案只会让用户逐渐对风险麻痹，这是该事件给我们上的其中一课。

![delete2-C3DJBD5P 大.png](Scenes%20Weekly%20%2350.assets/delete2-C3DJBD5P%20%E5%A4%A7.png)

{上图：Jakub 举例自家产品的对照}

→ 原文（注意 url slug 是 stardust🤭）

[How we lost 54k GitHub stars – HTTPie blog](https://httpie.io/blog/stardust)

---

10、同样悲催的是 Atlassian 经历了公司有史以来最长时间的宕机，官方称原因是服务器维护脚本对大概 400 名客户网站进行了不当的永久删除。Gergely Orosz 的[这篇文章](https://newsletter.pragmaticengineer.com/p/scoop-atlassian?s=r)整理事件全流程。文章后面，作者询问客户是否会因此不再使用 Atlassian 的产品，大多数人表示只要数据找得回来依然会继续使用，因为迁移成本太高了……此次事故对 Atlassian 最大的影响是稳定性声誉。[Linear](https://linear.app/cams-issues)的 CEO 趁虚而入，[表示](https://twitter.com/karrisaarinen/status/1513574249121812482)因为 Jira 受影响的团队来 Linear 可以白嫖任何付费计划一年😂。

---

10、Elan Kiderman Ullendorff 做了一个小工具 Scrubstack，它可以像 Wikipedia 的 random article 一样随机打开 Substack 上的文章。用 Elan 的话说就是，Scrubstack 可以让你体验到走进一个陌生人家里，从他的书架上随机拿出一本书的探索感。

→ 开始探索

[Scrubstack](https://lace-difficult-trombone.glitch.me/)

---

# 劳逸

![645d2acb33fc4c3fb9efd6aa8b20ea11.png](Scenes%20Weekly%20%2350.assets/645d2acb33fc4c3fb9efd6aa8b20ea11.png)

{上图：SFC 超级马里奥世界中，打败了 boss 同时堆出了 TAS 字样}

最近看 B 站 UP 主 [@冰连子](https://space.bilibili.com/169572934) 的 [TAS Metal Slug 系列](https://space.bilibili.com/169572934/channel/collectiondetail?sid=142321)终于打到了五代的最终关。也来分享下「云玩家」的快乐。TAS 早期指的是 Tool-Assisted Speedrun，借助工具的快速存档在低帧数下高精度地推进游戏，后来不单单追求竞速后，更具表演性质的 Tool-Assisted Superplay 开始流行，观赏性十足，也被用来挖掘一些正常流程看不到的 bug。

你可以在各大网站上搜索关键词查看更多视频。或者在 [TASVideos](https://tasvideos.org/) 按游戏查询 TAS 视频。

---

# 映像

现实拟像放映——

![9274aa06f2d44d14befc412fbf58cdb4.jpeg](Scenes%20Weekly%20%2350.assets/9274aa06f2d44d14befc412fbf58cdb4.jpeg)

{上图：微距下的百合花和水滴}

Daniel Olah 拍摄，摘于 Shot on iPhone [微距摄影大赛](https://www.apple.com.cn/newsroom/2022/04/apple-unveils-the-best-photos-from-the-shot-on-iphone-macro-challenge/)获奖作品。

---

写 newsletter 已有一年，本周在 V2EX 上发布了些许感想，作为一些改变的记录。

→ 原帖

[写了一年 Newsletter 后的些许感想 - V2EX](https://www.v2ex.com/t/846641)

---

喜欢本文的话，欢迎分享、订阅。

第 49 期请[在此查看](./Scenes Weekly #49.md)。

本次封面使用了 Familjen Grotesk 字体，不知道你有没有看到 ink trap……