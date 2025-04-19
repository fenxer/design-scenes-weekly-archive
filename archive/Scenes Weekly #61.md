# Scenes Weekly #61

2022-07-18

\> 设计视角下的世界——

第 60 期请[在此查看](./Scenes Weekly #60.md)。

本期出现：

- Arc 浏览器使用体验更新
- 长文本通知拆解
- 重读 HIG（二）
- 写在 Ev Williams 卸任 Medium CEO 之后
- 其他：交互界面历史、JWST & Hubble 照片对比、Weavve 项目关闭、会议语音辅助工具 Unblah、英语自动转正则 AutoRegex、DALL·E 2 Prompt Book、从政治学的角度看 web3 和 DAO、AI 新闻配图 PROMPT.PRESS、Figma 前端布局解析

如有格式异常建议点击最上方「在浏览器中访问」。

---

上周有读者指出，在 重读 HIG 一栏中，原文「iOS 16 中也把 Spotlight 直接变为点按触发」这句表述有误，实际情况是 iOS 16 下滑和点按都可以弹出 Spotlight，原文已做修改。其实仔细再读发现那一整段对这个例子的引用都不太准确，我的原意是想说，Apple 虽然没有把下滑刷新作为绑定手势，但是却尽量避免将其用为别的用途（比如 Safari 依然使用下滑刷新）。这样与上文承接有些不恰当，所以换了「另外」的说法。另在图标一节中，标题已改为「应用图标」。

欢迎上周的新订阅者们，感谢所有订阅者的支持。

---

# 杂事

1、Arc 浏览器更新： 已经用了近两周时间的 Arc 浏览器，再补充一些使用感受。

- 首先一个常见的 bug，就是无处不在的文本光标，仿佛每处文本都可以编辑一样，但其实只是一个闪烁的光标，无任何用途。不知道是不是我的个例；
- 目前 Acr 没有书签的概念（依然支持 chrome://bookmarks ），最接近的可能是常驻的文件夹。所以目前依然需要一个第三方书签管理，希望正式上线有所补全；
- 复制网址会去掉一些跟踪器，原本也是插件才实现的功能，省心；
- Split 布局在小尺寸屏幕上挺不友好的，需要宽屏；
- Split 更新后作为一个单独的标签页存在，不会影响其他网页。之前的逻辑太不清晰了；
- 对于中文系统来说，默认字体需要手动设置一下（ chrome://settings/fonts ），否则默认为宋体；
- 临时标签页（没有 Pin 也没有 Favorite）会在一定时间自动清除，默认 12 小时，最长 30 天，清除后可在 Archive 里恢复。相当于一个自动的 OneTab 插件；

![1670056993722.png](Scenes%20Weekly%20%2361.assets/1670056993722.png)

{上图：Archive 中自动关闭的标签可以一键恢复}

---

2、Growth Design 这期讲述了长文本的设计拆解。

![1670056998026.png](Scenes%20Weekly%20%2361.assets/1670056998026.png)

{上图：本期界面的重设计}

如上图，最右边是原本的长段文本，内容是 Québec Amber Alert 发布的儿童走失信息，它有很多值得注意的点：

- 文本很长，没有分段，阅读困难；
- 没有图像、地图等功能辅助；
- 警报消息类型很多；
- 点击无反应，不知道下一步操作是什么；
- 只能向左滑掉通知，之后不知道在哪里还能看到；
- 过于频繁的警报反而麻痹了群众，很多人开始对此视而不见，甚至屏蔽通知；

Dan 提议将文本解析成 iOS 16 新功能「实时活动」的形式，如上图左 1。并且可以展开（左 2）进一步查看详情和汇报等操作。实时活动顾名思义。当走失儿童被发现和找到时，都会更新卡片的状态。我对实时活动的原理还不太熟悉，🤔它会一直在锁屏底部吗（一般来说进程任务完成就会消失吧）？出现其他警报通知时怎么办？其他类型的通知使用什么排版呢（不是现有的模板会来不及发布一些紧急事项）？设计之外的一些事情目前依然存疑。

→ 查看原文

[Amber Alert Redesign: 5 UX Improvements That Could Save Lives](https://growth.design/case-studies/amber-alert-ux)

---

3、[Victor](https://twitter.com/vponamariov) 由于经常做一些奇怪的 UI Tips，已经被我拉进「人类观察」名单里（不接收其信息，只观察其活动）。上周他突然发布了交互界面历史的网站，收到不少好评。

网站梳理了从 1973 年 Xerox Alto 到 2007 年 OS X Snow Leopard 的界面变化。我最喜欢的果然还是 Mac 早期 System 系列的控制面板：

![1670056999802.png](Scenes%20Weekly%20%2361.assets/1670056999802.png)

{上图：Macintosh System 1 系统 Control Panel }

→ 回顾

[The History of User Interfaces](https://history.user-interface.io/)

---

# 重读 HIG（二）

本节是重读 Human Interface Guidelines 系列第二期，目的为温故知新和跟进新内容。 之后会专门整理。

## 颜色

- 颜色这节大多没什么值得再提的，依然可以看到 iOS 和 macOS 大量的语义颜色说明；
- macOS 要注意用户系统强调色带来的额外色板；
- 我个人不太熟悉，原来 watchOS 的系统背景是纯黑色（#000），意图是与屏幕外边框相融合，产生增大屏幕的错觉（手机深色模式同理）；
- 本节最后列出了 Apple 各平台系统颜色，有默认和高对比度两种；

→ 本节出自

[Color - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/color)

## 深色模式

- 少数情况下，可以考虑只提供暗色模式。比如增加观看媒体内容时的沉浸感（像直播、视频）；
- 上一节的系统颜色已经为深浅两种模式做了适配，SF Symbols 也是，搭配使用既省事又到位；

![1670057001603.png](Scenes%20Weekly%20%2361.assets/1670057001603.png)

{上图：iOS / iPadOS 默认三个层级背景}

- 要注意 macOS 的可选择额外的背景色，比如当用户勾选了「允许基于墙纸调整窗口色调」，一些窗口便会根绝墙纸更改颜色，但通常幅度很小。同时 Apple 也建议使用带有透明度的背景，窗口活跃时呈现墙纸的「背景模糊」（tinting）效果，不活跃时也可分辨为实色；

→ 本节出自

[Dark Mode - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/dark-mode)

---

# 摘录

这周看过的一些——

> How people speak is not how they write, and so what I edit toward in interviews is a subjectively true representation of the talking person—not a literally and objectively accurate record of the sounds coming out their mouth in the order they emerge. What I’m after is a written story that reads, sounds, and feels true to life for both reader and subject. And the best compliment I’ve gotten from many of my subjects (and those who know them) is that their interviews sound like themselves.

—— Chris Mohney - [What We Talk About When We Talk About People Talking About People Talking](https://strangework.substack.com/p/what-we-talk-about-when-we-talk-about)

---

# 小事

1、Medium 十年后，Ev Williams 卸任 CEO，这家以低门槛 UGC 内容生产起步的公司，还是迎来了新的一幕。

现在谈起 Medium 就像咖啡馆内偶然聊到的人生路人导师，现在不知在何处流浪，恰好新闻中有报道人家还活得好好的。当初的 Medium 依靠突出的体验设计塑造专注的写作体验，可分享的草稿功能让很多平台也为之受用，稳定的分发系统和强大的 SEO 优化让文章有更多的曝光机会。Medium 吸引的写作人群广度令人惊奇，那时候经常翻看 Medium 的设计文章，很多团队的博客和独立出版商也搬到 Medium 上发布（Custom domains for publications）。创作者只需写作，读者用户仅需订阅标签和关注创作者，就能收到源源不断的新内容——但这种美好仅限一时。

广告盈利模式打破了美好的幻想，标题党玩弄流量，大量低质内容充斥平台。比如 2015 年 Medium 点击量最高的十篇文章标题（大意）是：

- 欢迎来到 Medium
- 学习新事物的 37 个最佳网站
- 辞职创业让我的生活变得真 TM 好
- 每个人应该在早 8 点前做的 8 件事
- 科学证明，你需要停止做这 7 件事来提高效率
- 33 个网站让你变成天才
- 如何 4 步简单减肥
- 30 岁的我对 20 岁的我的建议
- 「应该」与「必须」的交叉路
- 7 个拒绝（注：这个是 Airbnb CEO Brian Chesky 分享的当初在硅谷以 10% 股份募集 15 万美元时，收到的 7 次回拒邮件）

逐渐我发现即便是自己关注的设计内容领域也有着不少水分，平台在这样的内容下，简洁的设计换了又换，首页过几周就有新样式，我曾经效仿的优雅的双层导航栏设计也早就不知所踪。2017 年，Medium 对 clickbait 终于忍无可忍，关闭了广告，实行全站订阅模式。

实际早在 2013、14 年，Medium 就在生产 PGC 内容，并依照点击或阅读时间付费给创作者。

Medium 的目标是创作者和订阅付费的飞轮增长：招募专业创作者生产高质量文章，来吸引订阅付费用户；更多的订阅代表创作者有更多的奖励分成，可以吸引更多的优质创作者和内容产出。我依然清晰地记得 /membership 页面的剪贴设计风格——

![1670057003593.png](Scenes%20Weekly%20%2361.assets/1670057003593.png)

{上图：2017 年末的订阅页面设计风格}

读者以 5 美元每月订阅后，根据 Claps 次数和其他参数按比例发放给创作者。普通用户依然可以选择免费发布文章（当然权重肯定会低一些，有阵子我的首页文章基本都带着星星），保持了一贯的低门槛和轻量的体验。然而问题在于：

- 作为优质创作者，为什么一定要来 Medium 创作而不是自立门户？
- 作为付费订阅者，为什么订阅后收到的是方方面面的内容？这些内容真的值得付费吗？我给了 每个喜欢的创作者 50 claps 后订阅的钱真的能给到每个创作者吗？

我印象里很长一段时间，外界都有唱衰 Medium 的声音，很多独立博主劝大家远离 Medium 这个中心平台。然而事实上 Medium 活得挺不错，2021 年初， Medium 声称有 72.5 万订阅用户，自己抽成 50%（对比 Substack 10% 真是惊人的数值…）获得 2100 万美元收入。

Nathan Baschez 指出小日子过得不错的 Medium 订阅有两个因素：

- 长尾（Long Tail）文章带来了巨大的搜索引擎渠道流量；
- 更高的分成。因为 Medium 身兼分发，平台本身具有价值，如同淘金地，发布内容就有可能赚钱。Substack 则不同，自己不去运营的话就会像本通讯一样默默无闻（它的 /Discover 依然和人气挂钩）；

Casey Newton 认为，高端出版平台被各大传统纸媒及其母公司控股的知名媒体占有，「低端」出版上，有 Substack 这种平台吸纳了很多个人品牌。Medium 处在了 Medium（中间）的位置，不上不下。待出版商们在 Medium 匿声后，Medium 又回到了依赖于搜索引擎的「大众杂志」。

Nathan Baschez 不同意 Casey 的看空，他觉得独立创作者只是概念上炒的火热，实际上大多数创作者未必喜欢身体力行。

- 首先可能只有真正的知名作家才能被称得上「独立」，不依赖平台就能获得社交资源；
- 独立创作需要前期投入，在没有正向的现金流之前，为了吃口饭不能 ALL-IN 写作；
- 有些创作者需要高端平台的身份证明，比如类似纽约时报评论员、The Atlantic 专栏撰稿人等头衔；
- 平台帮你处理写作以外的杂务；
- 平台分发机制；

上述特点在传统出版平台都能找得到，并且相当成熟。下一代互联网出版平台的方向是要挑选什么方向去对抗和进化传统平台，Substack 目前的分发机制和 iOS 的推出，在[第 46 期](https://designscenes.zhubai.love/posts/2117545871552929792#:~:text=%E5%88%9B%E5%A7%8B%E5%9B%A2%E9%98%9F%E6%98%AF%E8%A1%8C%E8%B5%B0%E4%BA%8E%E4%BA%A7%E5%93%81%E5%88%9D%E5%BF%83%E4%B8%8E%E5%88%A9%E7%9B%8A%E5%A2%9E%E9%95%BF%E7%9A%84%E7%8B%AD%E8%B7%AF%E4%B9%8B%E4%B8%AD)也有提到：「行走于产品初心与利益增长的狭路之中」。所以从这个角度看，Medium 还有机会，并非在苟延残喘。Baschez 希望在 Ev Williams 之后的 Medium 重新找到属于自己的驱动模式。

最近翻看 Medium 首页，发现又改回接近早期的首页结构了。

本小节结合了我的主观经历和以下信息参考。

→ Ev Williams 声明

[New Decade, New Ideas](https://ev.medium.com/new-decade-new-ideas-faee8e712589)

→ Did Medium Succeed?

[Did Medium Succeed?](https://every.to/divinations/did-medium-succeed)

→ Ev Williams gives up

[Ev Williams gives up](https://www.platformer.news/p/ev-williams-gives-up)

---

2、James Webb Space Telescope（JWST）这周传回了一系列惊人的图像，相信每一个热爱科学的人都为之振奋，JWST 「照亮」了宇宙更多的角落。有人在 GitHub 上传了 JWST 和哈勃望远镜的同星系对比图，差距颇大，可自由拖动查看。

![1670057005310.png](Scenes%20Weekly%20%2361.assets/1670057005310.png)

{上图：JWST 近红外相机拍摄的南环星云与哈勃拍摄图对比}

→ 网址

[Webb Compare](https://www.webbcompare.com/index.html)

---

3、每天收着 Google Analytics（GA）的 GA4 营销邮件，最近才发现 Analytics 在奥地利、荷兰、法国和意大利是非法的。

[Austrian Data Protection Authority](https://noyb.eu/en/austrian-dsb-eu-us-data-transfers-google-analytics-illegal) 最先禁用了 Analytics，原因是 GA 收集的数据会传输到美国，美国法律规定 Google 有义务根据要求向政府组织披露数据。随后其他一些欧盟国家纷纷开始禁用。

→ 来源

[Italy follows Austria, Netherlands, and France by banning Google Analytics](https://creativerly.com/google-analytics-illegal/)

---

4、[第 54 期](https://designscenes.zhubai.love/posts/2137824333849636864#:~:text=%E4%BC%9A%E6%84%9F%E5%88%B0%E7%96%B2%E6%83%AB%E3%80%82-,Weavve,-%E8%BF%99%E6%AC%BE%E6%96%B0)介绍了制作 PPT 的概念工具 Weavve，当时还在等待邀请的状态。结果上周创始人 Christian 发文说，不做了。

原因是在迭代版本时，Christian 开始质疑自己最初的产品目标。后来又发现了 Tome（[第 47 期](https://designscenes.zhubai.love/posts/2120066691403902976#:~:text=%E7%9A%84%20Storytelling%20%E5%B7%A5%E5%85%B7-,Tome,-%E3%80%82)有提到），与他的原型很接近，Christian 停止了思考。

接下来，他要和朋友去忙另一个项目。于是 Weavve 在没绽放前便枯萎了。

→ 官网原文

[weavve • The joyful alternative to Powerpoint and Google Slides](https://www.weavve.io/)

---

5、有些人开会总是一说就说个不停，不给其他人发言的机会。Unblah 是一个本地的语音记录工具。作者 Alexis Rondeau 的目的是缓解在网络会议上，自己发言过多或过少的情况。

![1670057007351.png](Scenes%20Weekly%20%2361.assets/1670057007351.png)

{上图：Unblah 正在记录语音状态}

如上图，在通过麦克风讲话时，Unblah 会记录语音时长（绿→橙）和语气停顿（空缺），来提醒自己讲话时长和流利程度。Alexis 特意在 FAQ 中提到，他不鼓励你拿这个应用去暗示那些话多的同事，他鼓励从自我做起，养成良好的会议发言习惯。

Unblah 完全免费，无需联网仅在本地运行。

→ 官网

[Unblah – For those (like myself) who often talk too much, or too little, in meetings because they get nervous](https://unblah.me/)

---

6、AutoRegex 是一个可以根据英语语句自动生成正则表达式的工具，一推出就大受欢迎，以至于开发者连夜上线了 $9.99 每月的付费计划，并把正则转英语功能列为收费项，效率真是高。

→ 试试

[https://www.autoregex.xyz/](https://www.autoregex.xyz/)

---

7、DALL.E 2 发布已有一段时间，[五月初](https://designscenes.zhubai.love/posts/2132756592087695360#:~:text=%E5%8D%95%E8%AD%A6%E5%91%8A.jpg-,DALL.E%202%20%E6%9B%B4%E6%96%B0,-%EF%BC%9A)我还在担心「设计奇点」的提前到来，两个月后我们智人种族就找到了驯服野生 AI 技巧。DALL·E 2 Prompt Book 这份文档详细地记录了如何使用各种关键词来生成特定风格图像，包含氛围、情感、摄影、电影风、插画风、艺术史、3D 艺术、编辑、合并图像等技巧。

![1670057010713.png](Scenes%20Weekly%20%2361.assets/1670057010713.png)

{上图：文档中利用不同镜头语言来调教 DALL.E 2}

→ 原文

[The DALL·E 2 Prompt Book](https://dallery.gallery/the-dalle-2-prompt-book/)

---

8、DAO 与实体政治对比，由于人群的提纯和小范围等特性，更像是亚里士多德所言的平民政体。平民政体建立在贫富平等的基础上，仅这一点便开始乌托邦化。作者主张最终还是要看智能合约的约束范围有多大多广和多深入。

→ 原文

[从政治学的角度看web3和DAO](https://mp.weixin.qq.com/s/cLy7WtARTsL0Q1xxy9-CNg)

---

9、PROMPT.PRESS 每天从各个新闻源摘取信息，然后依靠生成图像的 AI，把生成结果展示到网站上。不得不说，本来就有点魔幻的新闻标题，配上略显扭曲的非人工图像，反倒多了些夸张的真实。

![1670057013256.png](Scenes%20Weekly%20%2361.assets/1670057013256.png)

{上图：根据 "Elon Musk to Acquire Twitter" 事件生成的图像}

上图中的 Musk 带着一团不祥的黑雾，以一个奇怪的表情抱走变形的 Twitter 鸟，与现在的 Musk 大戏极其应景。 目前不清楚 David Jones 具体用的哪个 AI 引擎。

→ 网站

[AI generated artwork inspired by current events](https://prompt.press/)

---

10、Figma 右栏使用 Css Grid 布局，每列宽 8px，标准的 8pt-grid 布局。但对于设计师也到此为止了，接下来还是请前端大哥 Ahmad Shadeed 讲解 Figma 背后的布局。

![1670057014983.png](Scenes%20Weekly%20%2361.assets/1670057014983.png)

{上图：Figma 检查元素下的布局参考线}

→ 原文

[The CSS behind Figma - Ahmad Shadeed](https://ishadeed.com/article/figma-css/)

---

> 我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

→ [封面存档](https://figma.fun/f9e6Lk) ([figma.com](http://figma.com))

---

# 劳逸

![1670057021054.png](Scenes%20Weekly%20%2361.assets/1670057021054.png)

{上图：Sim CB 中的果农、果园和央行}

一款模拟央行的网页小游戏，你要做的只是调整利率，无需考虑其他商业银行，没有经济刺激政策，但要考虑平稳市场通胀，劳动力稳定，资源供需，最后在 240 月后结算生产总值作为游戏结果。对于宏观经济来说，已经是极其简化的模型，更多原理可以查看作者解释[原文](https://benoitessiambre.com/simcb.html)，涉及到果园运行机制、铸币税的重要性、罕见的负利率影响等。一个小 Tips 是，游戏里 Natural rate 并非严格指代现实的自然利率，而是利润最低的果园破产前能承受的最大利率约值，你的利率定的比这个数值高，就会有企业破产和失业率上升的风险。

→ 免费游玩

[Benoit Essiambre](https://benoitessiambre.com/macro.html)

---

# 映像

现实拟像放映——

![1670057022751.png](Scenes%20Weekly%20%2361.assets/1670057022751.png)

{上图：JWST 船底座星云 NGC3324}

IMAGE: NASA, ESA, CSA, STScI

→ [原图](https://webbtelescope.org/contents/media/images/2022/031/01G77PKB8NKR7S8Z6HBXMYATGJ?news=true)

---

# 温故

→ Scenes Weekly #12

[Scenes Weekly | No. 12](https://mp.weixin.qq.com/s/5vjMf5fZMMN5l2qYCGE38Q)

- Windows UI (Figma) 发布了 2.6 版本适配 Windows 11
- Product Hunt 和 GitHub Project 改版
- Google Search Console 推出 Search Console Insights
- I Love Typography 字体商店开张，并推出 CEDARS+ 字体筛选法
- Windows 窗口框架变迁
- Doodle Bugs 笔刷
- 音频社交关系链不对称
- 上世纪 IBM 海报计划
- 初识 GitHub Copilot
- Facebook 推出 Bulletin，与 Substack 和 Revue 竞争
- Twitter 官方账号戏仿 NFT 潮流

---

喜欢本文的话，欢迎分享、订阅。

第 60 期请[在此查看](./Scenes Weekly #60.md)。

本次封面使用了 MAZIUS REVIEW 20.09 字体，为本通讯新的标识。