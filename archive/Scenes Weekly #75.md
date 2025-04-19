# Scenes Weekly #75

2022-10-31

\> 设计视角下的世界——

第 74 期请[在此查看](./Scenes Weekly #74.md)。

本期出现：

- Twitter 被收购前
- Apple Watch 大都会表盘
- macOS Ventura 体验
- 重读HIG（十五）
- Twitter 用户兴趣转移
- 苹果 1984 年 Newsweek 广告
- AirPods 漏洞与苹果安全赏金升级
- 其他：iCloud 更新、App Store 广告堪忧、App Store 放行 NFT、98.css、Netflix 隔空投送营销、开源问答社区软件 Answer、MKBHD 观众 97% 为男性、Vercel 收购 Splitbee、Passkeys 科普、Wired 六词科幻小说活动归档、全景胡夫金字塔、The Crypto Story、AI 生成的矢量图、Stable Diffusion Hub

如有格式异常或邮件截断，建议点击最上方「在浏览器中访问」。

---

 Apple Week！

十月即将翻篇，北京还没有开始集中供暖，我怀疑自己正在失去恒温动物的特性，地球对面的 Elon Musk还在穿着短袖抱着水池走进旧金山 Twitter 总部大门。距离上次追剧 [Elon Musk & Twitter](https://designscenes.zhubai.love/posts/2158119020283875328#:~:text=%E5%B0%8F%E4%BA%8B-,Elon%20Musk%C2%A0%26%20Twitter,-%E8%BF%99%E5%9C%BA%E6%88%8F) 已有一段时间，总之就是总之那么回事，然而也有然而的事情发生了。

大意是，一直摇摆不定的 Musk 又能买下 Twitter 了，而且已经到了银行签署文件的时刻，130 亿债务融资基本板上钉钉。

![截屏2022-10-27 17.05.54.png](Scenes%20Weekly%20%2375.assets/%E6%88%AA%E5%B1%8F2022-10-27%2017.05.54.png)

{上图：以摩根士丹利为首的七家愿意相信 Musk 的银行。数据来源: Twitter SEC 文件，图表来源: Bloomberg}

Musk 答应银行家们会帮助他们把债券推销给基金经理，可能银行人士也和风投圈一样基于某种神秘的直觉认为，Twitter 虽然现在一团糟，但是还有救，Musk 的成功经验和魅力(?)能赋予 Twitter 新的前景——否则也不会像之前公开的交流信息显示，a16z 创始人 Marc Andreessen 愿意「无条件」为这场交易添砖加瓦 2.5 亿（实际投了 4 亿）。红杉资本也承诺提供 8 亿美元，合伙人 Roelof Botha 觉得 [Musk 很行](https://cn.wsj.com/articles/%E7%BA%A2%E6%9D%89%E8%B5%84%E6%9C%AC%E6%8E%8C%E9%97%A8%E4%BA%BAroelof-botha%E8%AE%A4%E4%B8%BA%E9%A9%AC%E6%96%AF%E5%85%8B%E6%94%B6%E8%B4%ADtwitter%E7%9A%84%E4%BA%A4%E6%98%93%E5%B0%86%E5%8F%96%E5%BE%97%E6%88%90%E5%8A%9F-11666752979)。虽然 Musk 说过在 Twitter 说过谈钱伤感情，但是 VC 们应该不能这么对 LP 说吧 (?)  440 亿美元真是不小的数目，它让 8 亿美元都显得有些微不足道。

→ [Bloomberg 新闻](https://www.bloomberg.com/news/articles/2022-10-25/musk-tells-debt-bankers-he-plans-to-close-twitter-deal-on-friday)

28日更新：他真的来了。[他说](https://twitter.com/elonmusk/status/1585619322239561728)：

> Low relevancy ads are spam, but highly relevant ads are actually content!

[Welcome to hell!](https://www.theverge.com/2022/10/28/23428132/elon-musk-twitter-acquisition-problems-speech-moderation)

最后让我们飞回寻常百姓家，欢迎上周的新订阅者，感谢所有订阅者的支持💸

---

# 杂事

1、Apple Watch 重新绑定新的 iPhone 需要重头做表，抹去所有数据并重新同步。也借此机会更换了一直在用的模块表盘。

![AW@2x.png](Scenes%20Weekly%20%2375.assets/AW@2x.png)

{上图：我使用的旧表盘为模块定制，新表盘为大都会定制}

虽然我很想用用[轮廓表盘](https://support.apple.com/zh-cn/guide/watch/apde9218b440/watchos#:~:text=%E5%87%BA/%E6%97%A5%E8%90%BD%EF%BC%89-,%E8%BD%AE%E5%BB%93,-%EF%BC%88%E4%BB%85%E9%99%90%20Apple)，但是小一圈的 S5 不支持。于是剩下的字体表盘中，大都会（Metropolitan）对我来说成了最好的选择。得益于拓展后成为可变字体的 [San Francisco 字体家族](https://developer.apple.com/videos/play/wwdc2022/110381/)，Apple Watch 的大都会表盘数字可以使用数码表冠调节至 16 种样式。打开「始终显示」设置后，抬腕唤醒时还有着优雅的过渡动效。

![Watch Face.jpeg](Scenes%20Weekly%20%2375.assets/Watch%20Face.jpeg)

{上图：大都会表盘从宽度和高度上调节的16种样式。图：Arun Venkatesan}

传统机械手表厚重的装饰主义让我敬谢不敏，我虽然不是某种简单风格的狂热爱好者，但是对包豪斯风格表盘毫无抵抗力，几年前在看某篇「红十二」介绍文章时，对 NOMOS 的「无国界医生」一见钟情， Tangente 和 Metro 系列都是我的心头好，和其他名表价格对比又不算太贵。

→ [包豪斯风格迷思](https://nomoswatchclub.com/bauhaus-watch-myth-en)

之前戴过的 [Tangente 101](https://nomos-glashuette.com/zh-hans/tangente/tangente-101) 是上图中第 2 排第 2 枚的偶数表盘结构（没有数字 6），字体轴为窄而高，我有即兴做过该字体的[奇数字体版](https://twitter.com/haxfenx/status/1255405198815756288)。这次重新用回传统表盘选择了宽而矮的全数字风格，以形成一种圆环的感觉。

→ 查看 Arun Venkatesan 对该表盘的[介绍](https://arun.is/blog/apple-metropolitan-face/)

---

2、这周除了更新 iOS 16.1，Windows 22H2，还更新了 macOS Ventura。我可能就是图那个 Live Text 加入日语语种识别（当然还有一些安全更新，后面会提到）。

最大的功能更新台前调度有点没用明白……我没有找到比起现在多桌面有什么优势。而且进一步压缩了 MBP 可怜的屏幕宽度，Arc 浏览器里实际展示的网页宽度都快突破 1280px 断点了😅，还不如 Windows 笔记本的 1366 宽度。 虽然左侧各个应用缩略图是实时更新的，但返回桌面后拖动文件到该程序上却没有反应。倒是 iPad 上的原神玩家对这个功能很喜欢，直呼[库克你是懂原神的](https://www.bilibili.com/video/BV12e4y1e7xc/)。

新的系统偏好设置——哦不对，现在是「系统设置」——简直是灾难。

![network.png](Scenes%20Weekly%20%2375.assets/network.png)

{上图：Ventura 13.0 中网络和 Wi-FI 设置作为父子关系却分别有入口}

这个层级安排给我整不会了，网络设置继承自旧系统，Wi-Fi 设置又沿袭自 iPadOS，作为父子层级却又因此都有单独的入口，爱走迷宫是吧？

![Setting icons.png](Scenes%20Weekly%20%2375.assets/Setting%20icons.png)

{上图：左边为 iOS 设置控制中心截图，右边为 Ventura 辅助功能菜单截图}

再看图标一列也是不忍入目。macOS 的特色阴影在这里发挥得并不好。背景也没忘记使用渐变样式，深色模式下这些黑色背景的图标显得尤其辣眼睛。而且在 iOS 上更早出现的深色模式图标，到 Ventura 上变成了外观设置，迷惑。

![MENU BAR.png](Scenes%20Weekly%20%2375.assets/MENU%20BAR.png)

{上图：左边为 Monterey 程序坞与菜单栏设置截图，右边为 Ventura 控制中心截图}

Monterey 中偏好设置中最喜欢的菜单栏设置界面现在已经消失，如果说其他地方多少带些不熟悉的感觉在吐槽，但是这里已经是明显的倒退，变得非常不直观。

→ 更详细的批评可以回顾 Jeff Johnson 的[文章](https://lapcatsoftware.com/articles/SystemSettings.html)（有两部分）。

![FONTBOOK-2.png](Scenes%20Weekly%20%2375.assets/FONTBOOK-2.png)

{上图：Ventura 新的字体册截图}

字体册加入新的视图，优化了字体展示信息。但是字体缺省文本改为了「那只敏捷的棕毛狐狸跳过那只懒狗，消失得无影无踪」，而且不知为何一些英文字体无法转换到「棕狐跳懒狗」的英文版。

然后不知为何 macOS 的预览[不再支持查看 PostScript 文件](https://www.macrumors.com/2022/10/25/macos-ventura-preview-app-drops-postscript-support/)（包括 .ps 和 .eps ）。

最后推荐一下 Ars Technica 的[全面评测](https://arstechnica.com/gadgets/2022/10/macos-13-ventura-the-ars-technica-review/)。

---

# 重读HIG（十五）

本节是重读 Human Interface Guidelines 系列连载第十五期，目的为温故知新和跟进新内容。 为避免篇幅过长，不会一次发布太多，之前内容已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上。

## 模态（Modality）

对于这个你可能习以为常的翻译术语，在本节开头有一段像 *The Declaration of Independence* 的模态定义，如下拆解。

- Modality is a design technique.
    - 模态是一种设计技术/技巧/工艺。
- Modality presents content in a separate, focused mode.
    - 模态以单独、专注的模式呈现内容。
- Modality prevents interaction with the parent view.
    - 模态可以阻止与父视图交互。
- Modality requires an explicit action to dismiss.
    - 模态需要一个明确的交互退出。

这种特定的模式状态可以确保用户收到重要的信息，提供确认选项或专注于复杂任务的一部分。虽然它的形式不止于弹窗，但是为了方便理解可以选择一种自己熟悉的形式。

- 模态会打断当前流程体验，有必要再使用；
- 保持模态任务的简洁性，有助于快速完成这一块任务；
    - 如需要沉浸感可以进入全屏模式；
- 模态的形式设计不要造成 app 中 app 的错觉；
    - 也不建议叠加模态中的模态；
- 有明确的交互提示关闭模态。有必要的话关闭时给予确认选项避免数据丢失等容错；

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/modality)

## 多任务（Multitasking）

题外话：我对智能移动操作系统一个很大的感受是，隔壁 S60v3 可以后台程序进行多任务处理，俺们那儿 S40 就不行。当时在艾网（agrj）学着在 J2ME 中漫游，对于 QQ 等软件的后台化便已经是多任务追求的终点。

多任务的执行大多是系统层面的事情，所以 HIG 这节介绍了各个平台上的多任务模式。

在 Best practices 一段，有点像是之前「全屏」一节中的注意事项：

> 📮回溯：[全屏（Going full screen）](https://www.craft.do/s/fH49oLBCFdJO4l/b/CAD17A65-426F-4FC6-B92A-F092E62E1D5E/%E5%85%A8%E5%B1%8F%EF%BC%88Going_full_screen%EF%BC%89)

> 一些应用离开全屏时，可以默认帮助用户暂停当前流程。比如游戏或者视频。视频的话还可以选择继续背景播放或自动变为画中画，游戏也可以有不暂停但降低帧率等优化选项。当然还有一些「明显的」应用就不必了，比如下载器、音乐播放等。具体场景具体考虑，原文并没有说清楚这一点。

在所有平台中，iPad 的多任务处理又最特殊。基本分为分屏浏览、侧拉和画中画。

![截屏2022-10-25 15.36.06.png](Scenes%20Weekly%20%2375.assets/%E6%88%AA%E5%B1%8F2022-10-25%2015.36.06.png)

{上图：iPad 上两种多任务处理}

iPadOS 13 中，iPad 率先在 Safari 引入窗口概念，详情可观看 [WWDC19 视频](https://developer.apple.com/videos/play/wwdc2019/212/)。对于操作方法，苹果的[用户支持](https://support.apple.com/zh-cn/HT207582)也有很详细的说明。

iPadOS 15 及其更高版本中可以指定这种窗口的形式：

- Prominent：突出式。一个处于屏幕中央的模态窗口，周围会变暗以呈现当前主要任务（比如邮件应用中，长按侧栏邮件弹出的窗口）；
- Standard：标准式。分屏显示的窗口，特点是每个窗口功能一致，都可以实现 app 的所有功能（比如 Safari），Prominent 则不能；
- Automatic：系统根据交互上下文自动设置；

HIG 建议：

- 用户可在 Prominent 窗口独立完成任务，而不用呈现 app 所有的功能；
- 同样不要滥用窗口，仅在需要或者用户明确时使用窗口；
- 多窗口虽然层次清晰，但是不应独占某项功能，主窗口依旧可以完成所有任务；
- 维持窗口状态；
- ……

更多内容请查看原文。

值得一提的是 HIG 没有提及 Ventura 台前调度新功能。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/multitasking)

---

# 摘录

这周看过的一些——

> the bird is freed

—— Elon Musk - [Twitter](https://twitter.com/elonmusk/status/1585841080431321088)

---

# 小事

3、路透社：Twitter 内部对「重度 Twitter 用户」的评定标准是每周登录 6 或 7 天，并且每周发布 3 到 4 次推文的人 。

这份 *Where did the Tweeters Go?* 内部调查报告表示，Twitter 活跃度最高的英语用户现在对加密货币和 NSFW 内容最感兴趣。之前[介绍过](https://www.theverge.com/23327809/twitter-onlyfans-child-sexual-content-problem-elon-musk) Twitter 虽然对 OnlyFans 模式很感兴趣，但是没法解决儿童色情问题。而新闻、体育和娱乐兴趣正在减弱——这是广告商最不想看到的。

名人效应和电子竞技相关内容兴趣也在下降，哦——

→ [原文](https://www.reuters.com/technology/exclusive-where-did-tweeters-go-twitter-is-losing-its-most-active-users-internal-2022-10-25/)

---

4、苹果买下了 1984 年新闻周刊（Newsweek）的所有广告版面用于宣传第一台 Mac，Macintosh 128K。苹果在第一面广告上写到：

> According to Apple, the reason is simple: using a Macintosh is “easier than falling off an IBM user manual”.

![too.png](Scenes%20Weekly%20%2375.assets/too.png)

{上图：广告中的鼠标指南}

虽然这次 Macintosh 试用活动效果并不好，但也有 20 万人参与。由于 Macintosh 的个人电脑定位，苹果必须让大众知道鼠标和 System 1.0 系统的奇妙之处，Apple Garamond 字体承担了大部分责任。苹果还推出了 [Macintosh Guided Tour](https://www.youtube.com/user/Mac128DOTcom/videos)（400K软盘）帮助用户学习，今天来看都很有意思。

→ [归档](https://guidebookgallery.org/ads/magazines/macos/macos10-newsweek)

---

5、[AirBuddy 2](https://v2.airbuddy.app/) 的开发者 Guilherme Rambo 在测试 AirPods 连接时发现了一个严重的漏洞，该漏洞可以通过任意拥有蓝牙权限的应用，在你使用无线耳机（AirPods、Beats）时，记录你与 Siri 或者 iOS 听写功能期间的语音，此过程不会留下任何调用麦克风的记录。在 macOS 上也可绕过 TCC（Transparency, Consent, and Control）控制，向 DoAP 服务请求音频数据。

Rambo向苹果安全团队报告了这个问题，并在 16.1 等一系列新系统发布时修复。10 月 25 日，他获得了 7000 美元「赏金」。

这段故事完结了。但在 27 日，苹果安全团队发布了一条 *[Apple Security Bounty Upgraded](https://security.apple.com/blog/apple-security-bounty-upgraded/)* 的文章。

苹果表示，自 2016 年该计划启动后，已经向相关系统研发人员提供了近 2000 万美元赏金。此次升级，苹果安全团队加快了报告反馈速度，研发人员也更容易向苹果提交报告，还细化了[各级别漏洞赏金](https://security.apple.com/bounty/categories/)。甚至你[可以申请](https://security.apple.com/research-device)一个很酷的 Security Research Device（SRD）。

![SRD.png](Scenes%20Weekly%20%2375.assets/SRD.png)

{上图：Apple Security Research Device}

在这台特殊的 iPhone 上你可以访问系统 Shell，运行各种工具，甚至自定义内核。租期 12 个月，且过去一年内未在苹果就职，还有着严格的地区限制。

Rambo提供的漏洞看起来并不像最低档 5000 美元级别，然而就是晚了两天？

---

5.1、网页版 [iCloud](https://beta.icloud.com/) 主页界面更新，可以自定义主页。查看照片时也有着和 iOS 类似[照片信息](https://twitter.com/_patmurray/status/1585386493417119744)弹窗。云上贵州还没有更新。

5.2、App Store 新加入的广告质量低下，[引人不满](https://www.theverge.com/2022/10/26/23424316/app-store-gambling-ads-listings-apple-developers)。同时允许开发者有限制地 mint、转让 NFT，当然也要收过路费，看来 iOS 16.1 带来了更多[之外的信息](https://techcrunch.com/2022/10/25/apple-cracks-down-on-nft-functionality-social-post-boosts-with-app-store-rules/)。

5.3、作为新新拟物，Windows 98 给浮雕带来了大量设计就业。[98.css](https://jdan.github.io/98.css/) 可以带你回到那个时代。

5.4、十月初，[Netflix](https://www.marketingbrew.com/stories/2022/10/17/promotion-tactics-for-netflix-s-adaptation-of-stephen-king-s-mr-harrigan-s-phone-include-airdropping-thousands-of-passerby) 在广告牌附近使用隔空投送（AirDrop）功能宣传新片 Mr. Harrigan's Phone（哈里根先生的手机），同时在 Google 买好关键词，以引流到新电影中。

5.5、思否团队最近开源问答社区软件 [Answer](https://answer.dev/)，作为曾经的 Typecho 用户支持一下。

5.6、[MKBHD 说](https://twitter.com/julesterpak/status/1583711388958326784)他的订阅受众性别分布为，97% 为男性，3% 为女性。

5.7、Vercel 收购了隐私先行的统计工具 [Splitbee](https://vercel.com/blog/vercel-acquires-splitbee)，这类工具通常使用不同的统计方法，比如流量趋势。

5.8、WWDC22 苹果推出 Passkeys 以取代手动输入密码，Windows 和 Android 也预计在 2023 年第一季度支持。[Passkeys.io](https://www.passkeys.io/) 这个网站科普了其原理，并且可以亲自体验一下完整地使用 Passkeys 注册登录流程。

5.9、Wired 每月都会举办 *#WIREDSIXWORD* 活动，征集六个单词写出的科幻小说，选出的优胜位会配上一副精致的插图，[这里是一些归档](https://www.wired.com/story/six-word-sci-fi/)。

5.10、你不应该错过这个胡夫金字塔的全景[介绍网站](https://giza.mused.org/en/guided/266/inside-the-great-pyramid)。

5.11、你更不应该错过 [Matt Levine](https://www.bloomberg.com/opinion/authors/ARbTQlRLRjE/matthew-s-levine) 这篇 [The Crypto Story](https://www.bloomberg.com/features/2022-the-crypto-story/)，他在 Elon Musk 以外的话题写了四万字！

5.12、AI TIME——[VectorArt.ai](http://VectorArt.ai) 里面都是 AI 生成的矢量图，不过看起来很像是生成位图转化的。

5.13、[Stable Diffusion Hub](https://stablediffusionhub.com/) 提供了各种 SD 训练模型（包含 NSFW）。

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

![BAYONETTA3.png](Scenes%20Weekly%20%2375.assets/BAYONETTA3.png)

{上图：Bayonetta 3}

整个 10 月都有很多游戏，之前推荐的[最后指令](https://store.steampowered.com/app/1487270/?snr=1_wishlist_4__wishlist-capsule)和 [SIGNALIS](https://store.steampowered.com/app/1262350/SIGNALIS/) 都是特别好评，[女神异闻录5皇家版](https://store.steampowered.com/app/1687950/5/)仿佛回到了刚发售时期，[星之海洋 6](https://store.steampowered.com/app/1776380/STAR_OCEAN_THE_DIVINE_FORCE/) 系列重启再遭冷，[骑马与砍杀2：霸主](https://store.steampowered.com/app/261550/Mount__Blade_II_Bannerlord/)和[吸血鬼生存](https://store.steampowered.com/app/1794680/Vampire_Survivors/)都迎来了正式版，我趁着被 Steam 发放日区买了*[新美妙世界](https://store.steampowered.com/app/1647550/NEO_The_World_Ends_with_You/)*。这些游戏都有一个共同的特点，我都还没玩过，F**K。当然也包括 Bayonetta 3，但我打算之后有时间从 1 开始玩起。

---

# 映像

现实拟像放映——

![Dupre4.jpeg](Scenes%20Weekly%20%2375.assets/Dupre4.jpeg)

{上图：使用纸和剪刀拼贴的柴犬肖像}

© [Lola Dupre](https://loladupre.com/) 

---

# 温故

→ [Scenes Weekly #26](https://www.craft.do/s/YNdfyUwCkh91p2/b/27F2804E-B87C-4350-A9D5-99F58C3A4E17/Scenes_Weekly__26)

- Windows 11 音量调节信息减少
- LoveFrom 官网上线
- PowerToys 重设计
- LGBTQIA+ 社区 Serif 重新设计标识
- 多邻国 S-1 文件解析
- Figma 固定选区
- Hopper 应用评测
- Stripe Press 上线
- 网格渐变生成工具 Mesh Gradient Tool

---

喜欢本文的话，欢迎分享、订阅。

第 74 期请[在此查看](./Scenes Weekly #74.md)。

本次封面使用了 SF Pro Display 和 SF Pro Text 字体，使用了 SF Symbol 图标。