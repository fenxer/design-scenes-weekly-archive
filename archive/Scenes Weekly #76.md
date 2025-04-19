# Scenes Weekly #76

2022-11-07

\> 设计视角下的世界——

第 75 期请[在此查看](./Scenes Weekly #75.md)。

本期出现：

- 重读HIG（十六）
- Bill Gates 用赛博邮票打击 spam
- Darin Fisher 加入 Arc 团队
- Safari 16.1 新功能
- 其他：The Uncomfortable 展示、订阅墙统计、iA Presenter、Affinity 大新闻、论文解释器 Explainpaper、Generator of random awesomeness、Twitodon、新社交应用 Gas、AI 伦理讨论还在继续

如有格式异常或邮件截断，建议点击最上方「在浏览器中访问」。

---

苦乐并存，复杂的一周。由于周末糟糕的加班（加班也分评级），我脑海中数次闪过这期鸽了的想法，但还是想坚持一下。

这期不会有太多文字，又是充满链接🔗的一期。

欢迎上周的新订阅者，感谢所有订阅者的支持🫡

---

# 重读HIG（十六）

本节是重读 Human Interface Guidelines 系列连载第十六期，目的为温故知新和跟进新内容。 为避免篇幅过长，不会一次发布太多，之前内容已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上。

## 新用户引导（Onboarding）

新用户的引导应该是简洁、轻快的，不用提供太多太复杂的信息，特别是没有专业的设计师帮你优化 PM 式啰嗦文案的时候。

如果应用想要获得一些隐私相关的权限时，可以在引导流程合适的阶段向用户展示其好处或用途是什么。 

比起图文式展示，交互式引导用户更好一些：

- 让用户感知到他们已经用上该应用了；
- 一些复杂应用中更容易说明引导；
- 更有助于记忆，所谓好记性不如烂笔头；
- 这种引导可以很灵活，不一定要引导用户一次体验所有功能，在用户遇到哪种功能需求时再说明也不迟；

> 💡拓展：之前在 Mobbin 看到过一个应用叫 [Demo](https://mobbin.com/apps/demo-ios-7a8528b2-6f36-4663-bf1d-f4dc83ebf5dc/e21859ac-3484-42a9-9908-a669f2b84f58/screens)，该应用的目标是让人无需乐器和乐理知识便可编曲和填写歌词，做出属于自己的歌曲。降低音乐制作门槛不是那么容易的事，它的 onboarding 流程足足有 31 屏。

如果你提供类似上述的引导教程，别忘记加上跳过操作。

除了必要的，大多许可信息也不必加到引导流程中。可以放在 App Store 页面或者设置关于等地方。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/onboarding)

## 触感（Playing haptics）

除了视觉和[听觉反馈](https://developer.apple.com/design/human-interface-guidelines/patterns/playing-audio)，系统还提供触感反馈。iOS 不必说，macOS 有 Force Touch 模拟反馈，类似 Apple Watch 旋转数码表冠。

就像看到红色就联想到错误信息、看到 switches 控件就想到功能开关控制一样，使用触感也需要赋予其因果信息，凭空使用触感很容易让用户迷惑。

和其他反馈一起使用效果可能会更好，比如一些音效出现时的震动。

频繁的触感会使人厌烦（说得好，所以我关闭了 iOS 键盘触感反馈），同时也要提供关闭触感的设置选项。

> ⚠️警告：慎重使用高强度触感。确保不会对摄像、麦克风和陀螺仪有影响。

你当然可以自定义触感，HIG 将其分为两个基本模块：

- 短暂的事件：短时间急促地震动一下，像是轻拍或脉冲那种感觉；
- 持续的事件：较长时间地维持震动，比如某些游戏中的激光特效；

对于震动触感本身，一般用锐度（sharpness）和强度（intensity）两个维度定义。前者用来控制震动是否柔和，后者则是顾名思义控制震动强度。我不懂开发实现，感觉可以暂且看成简谐振动中的周期和振幅参数？

触感的最好的体验方法，还是去找个应用或游戏亲自体验一下。如果有 PS5，更推荐使用 DualSense 体验细腻入围的震动体验，相信会有所启发。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/playing-haptics)

---

# 摘录

这周看过的一些——

> Card games are fun in large part due to their variance. Each game playing out differently is what separates it from games like Chess, which play out so similarly that often players memorize long series of opening plays and counter-plays.

—— Ben Brode - [Twitter](https://twitter.com/bbrode/status/1584762937477976064)

---

# CHILL

1、2004 年初，Bill Gates 承诺垃圾邮件问题将在两年后消失。Hotmail 的做法除了类似白名单和人工验证的机制外，还引入一种机制：给陌生人发邮件需要带上邮资（赛博邮票），如果收件人收到后认定你是在骚扰，那么收件人有权没收邮资，来大大增加垃圾邮件发送成本；如果你发现对方是失联多年的亲兄弟，那么你可以退回该邮资。

彼时雅虎邮箱也对这方法[很感兴趣](https://www.neowin.net/news/gates-backs-e-mail-stamp-in-war-on-spam/)，但由于大众的反对仅半年后微软便废黜了这一规则。向所有邮箱使用者无差别收费是不恰当的，本末倒置地抹去了互联网便宜好用的沟通交流特点。

Gates 还讨论了对发件人身份认证的可能性，包括缴纳一些「认证费」来确保你的邮件不会被识别为垃圾会话。一旦你发送了垃圾邮件，违反了规则，微软就会直接没收这些担保认证费。

Musk 和 Gates 的关系[一直不太好](https://www.cnbc.com/2022/05/05/bill-gates-says-elon-musk-could-make-twitter-worse.html)，但有些想法却颇为类似——每月 8 美元就能让我的垃圾言论镀金为认证自由言论，是不是反倒应该谢谢 Musk 呢？

→ [原文](https://www.bloomberg.com/news/newsletters/2022-11-03/elon-musk-s-twitter-blue-sounds-a-lot-like-bill-gates-s-plan-to-charge-for-email?cmpid=BBD110322_TECH)

Oh，本期应该不会出现 Musk 新闻了。



2、曾经的 Netscape 工程师，创造了 Firefox、Chrome 的 [Darin Fisher](https://www.linkedin.com/in/darin-fisher-7059ab/) 加入了 The Browser Company（原本是顾问）。在 [The Verge](https://www.theverge.com/2022/10/31/23428862/arc-browser-web-company-darin-fisher) 这篇新闻稿中，Fisher 也提到了iOS15 Beta 时期 Safari 的巨大改动，即把地址栏挪到底部引起了（仅仅是）测试用户的巨大反感，他认为在大公司高用户数产品中做优化创新已经很难，这也是近几年 Chrome 外观和交互几乎没有改动的原因。

![截屏2022-11-05 16.22.13.png](Scenes%20Weekly%20%2376.assets/%E6%88%AA%E5%B1%8F2022-11-05%2016.22.13.png)

{上图：文字 I’m helping build the browser of the future again - Darin Fisher}

对于 Google 来说，Chrome 团队的核心任务并不是打造优秀的浏览器，而是为保持 Google 搜索引擎的占有率，所有功能（包括创新）都无法绕开这一公司营收点，导致团队虽然有很多好想法但无法落地——毕竟把标签页设计的太容易管理，用户就没法再打开 Google 搜索一次关键词进入某个网站了。

新闻稿中似乎还能看到，Fisher 也参与了Arc 浏览器的基础构建。未来为移动端设计浏览器依然是一个巨大的挑战，

→ [原文](https://www.theverge.com/2022/10/31/23428862/arc-browser-web-company-darin-fisher)

另一个好消息是，Arc 在几个月后即将登陆 Windows 系统，将会使用 [Swift](https://www.swift.org/blog/swift-on-windows/) 带来纯原生的 Fluent Design 体验。酷！
→ [介绍视频](https://www.youtube.com/watch?v=bOMQiMxh5Bc)



3、Safari 16.1 现在支持： 

- web 通知推送
- AVIF 图片格式支持
- Passkeys 支持
- [Scroll to Text Fragment](https://wicg.github.io/scroll-to-text-fragment/) 支持，但不像Chrome 能手动复制。本通讯大量使用了该特性
- ……

→ [更多功能](https://webkit.org/blog/13399/webkit-features-in-safari-16-1/)



4、The Uncomfortable 是 Katerina Kamprani 一个专门用来展示日常生活中，一些物品变得让人不舒服会是什么样子。

![key_01_p.jpeg](Scenes%20Weekly%20%2376.assets/key_01_p.jpeg)

{上图：THE UNCOMFORTABLE KEY}

→ [网站](https://www.theuncomfortable.com/#)



5、Toolkits 和[National Research Group](https://www.nationalresearchgroup.com/) 对具有代表性的 2509 名美国消费者调查显示，53% 的人试图绕过新闻网站的订阅付费墙（paywall）。

→ [更多思考](https://toolkits.com/subscription-publishing/research-bypassing-paywalls/)



6、让我们数数一共有几个新型演示文稿工具了，Tome、Chronicle、Gamma，现在 iA 也推出了 [Presenter](https://ia.net/presenter)。Markdown 转 slide 工具[已不鲜见](https://gist.github.com/johnloy/27dd124ad40e210e91c70dd1c24ac8c8)，但他是 iA 出品。



7、Affinity 将在 11 月 9 日宣布 “[Something BIG](https://affinity.serif.com/zh-cn/?mc=V2_LAUNCH_EMAIL)”，拭目以待。



8、Explainpaper 使用 AI 帮你看懂一些晦涩的论文究竟在讲什么。

![截屏2022-10-31 16.05.38.png](Scenes%20Weekly%20%2376.assets/%E6%88%AA%E5%B1%8F2022-10-31%2016.05.38.png)

{上图：试用论文 Can we use algorithms to choose type}

目前只支持英语论文。如果你之前看到过这个网站——这周他们完善了一下界面设计。

→ [网站](https://www.explainpaper.com/)



9、Google 搜索的「手气不错」已经名存实亡，但还有 [Generator of random awesomeness](https://sharkle.com/) 想给你随机带来有趣的项目。



10、[Twitodon](https://twitodon.com/) 可以让你在 Mastodon 上寻找 Twitter 的朋友们。



11、Chrome 在 110 及后续版本移除 [JPEG-XL](https://jpeg.org/jpegxl/) 支持，该功能启用之前一直藏在 //flags/ 设置里。但 Chrome 方面表示整个行业生态对 JPEG-XL 没兴趣，比起现有的格式（比如在推广的 WebP 和 AVIF）没有足够的优势。

显然这种[模糊的说法](https://www.phoronix.com/forums/forum/software/general-linux-open-source/1354972-google-outlines-why-they-are-removing-jpeg-xl-support-from-chrome)无法服众。



12、前 Meta 产品经理推出了新的社交应用 [Gas](https://apps.apple.com/us/app/gas/id1641791746) 直逼 TikTok 和 BeReal 势头，看了一圈感觉有些像 QQ 之前的老功能「坦白说」。



13、[第 68 期](https://designscenes.zhubai.love/posts/2178446713948692480#:~:text=%E6%9C%88%2029%20%E5%8F%B7-,mimic,-%EF%BC%88%E3%83%9F%E3%83%9F%E3%83%83%E3%82%AF%EF%BC%89%E5%85%AC%E5%B8%83%EF%BC%8C%E5%BC%95%E8%B5%B7)介绍过 AI 生成项目 mimic 带来的争议。10 月初在韩国漫画家金政基（Kim Jung Gi）的意外离世几天后，有人把他的作品「投喂」学习让 AI 生成更多的类似风格作品，同样引起了群众反感。

AI 生成技术上层是从艺术家那里剥夺风格而不带有灵魂，下层是为中底层可复现工作的劳动者带来失业恐慌。以知识产权闻名的东京律师事务所 TMI Associate 提到，2018 年日本立法机构修改了「版权法」，规定机器学习模型允许从互联网抓取未授权的图像进行学习，这也是 [NovelAI](https://novelai.net/) 立足之处。

关于 AI 生成项目的伦理讨论还在继续，[第 74 期](https://designscenes.zhubai.love/posts/2196164196608143360#:~:text=GitHub%C2%A0Copi%C2%ADlot%C2%A0inves%C2%ADti%C2%ADga%C2%ADtion)提到的 GitHub Copi­lot inves­ti­ga­tion 现在进展到[正式提起诉讼](https://githubcopilotlitigation.com/)阶段。

→ [原文](https://restofworld.org/2022/ai-backlash-anime-artists/)

---

# 劳逸

![1500x500.jpeg](Scenes%20Weekly%20%2376.assets/1500x500.jpeg)

{上图：Marvel Snap}

大部分知名 IP 改编的游戏会像 [Marvel’s Avengers](https://store.steampowered.com/app/997070/Marvels_Avengers/)、[Marvel vs. Capcom: Infinite](https://store.steampowered.com/app/493840/Marvel_vs_Capcom_Infinite/) 一样褒贬不一，不过 [Marvel's Guardians of the Galaxy](https://store.steampowered.com/app/1088850/Marvels_Guardians_of_the_Galaxy/) 倒是不错。Marvel Snap 便是属于后者，

它是前炉石传说总监 Ben Brode 独立后的工作室第一部作品，这位炉石玩家最熟悉的设计师用了四年制作出一款精致的卡牌游戏。Snap 吸取了诸多炉石和 [Artifact](https://store.steampowered.com/app/583950/Artifact/) 等游戏元素，并大幅度简化。

简单说，你要和你的对手拔河，只不过有三条绳子。六回合打牌（视情况），最后看谁能拔过对面至少两条绳子。没有法术牌，每条绳子你最多只能放置四位英雄去拔，同时每条绳子自身也有随机附加效果以中和套牌（12张）带来的确定性。如果是打天梯，还可以和对手玩上一局德州式赌局——SNAP 加倍下注你的天梯等级。游戏的卡牌获取路线也是固定的，但是不同玩家之间是随机的，对非氪金很友好（当然要付出时间）。

1 分钟上手，5分钟一局。将碎片化时间利用到了极致。推荐。

目前可在外服移动应用商店和 [Steam](https://store.steampowered.com/app/1997040/MARVEL_SNAP/) 免费开玩。

---

# 映像

现实拟像放映——

![coApvOqBLOdSURMA7xU696fijCHfqOOt.jpeg](Scenes%20Weekly%20%2376.assets/coApvOqBLOdSURMA7xU696fijCHfqOOt.jpeg)

{上图：无人机拍摄的冰岛法格拉达尔火山最后的喷发阶段的裂缝}

**Big Bang**

© Armand Sarlangue

---

# 温故

→ [Scenes Weekly #27](https://www.craft.do/s/YNdfyUwCkh91p2/b/9B7BD344-B33B-4F8D-856A-3355E3F014D4/Scenes_Weekly__27)

- Product Hunt 改版
- 新 Macbook Pro 刘海屏下的 HIG 新改动
- 兔小巢反馈社区出探适老化与无障碍改造
- Windows 3.1 icons
- Literary Hub 经典书籍封面
- Figma Schema 大会
- 支持VR/AR 查看的 MorphCharts
- iOS 全角标点输入 Bug
- Share a secret 一次性加密文本发送工具
- 玩具厂商 McMiller 品牌字体 Doughy
- Adobe 替代产品展示网站 ADOBE SUCKS
- 排名前 10000 的网站 favicon 统计

---

喜欢本文的话，欢迎分享、订阅。

第 75 期请[在此查看](./Scenes Weekly #75.md)。

本次封面使用了 Kokoro（Trial）字体。