# Scenes Weekly #15

2021-07-25

本系列为微博 @Design_Scenes 的每周总结以及其他杂事。

本周出现：适老化、Safari、Apple Style Guide、Tweet Deck、mobbin.design、a11y、Morning Brew、Apple、Twitter、Fast Company、Godly Website、Airpods、HEIC、Macintosh Guide、Piedmont Art Walk、Honk、Billion Dollar Pitch Deck、50+ AI tools、Audubon Photography Awards、Paint Up、Telsa、Google Doodle、Chrome Dino、Clubhouse、Mapbox Studio、斗鱼追光体、Tricycle、meme

---

# **周日**

下图为工信部《互联网应用适老化及无障碍水平评测体系》截图，主观受众人群和客观自动化检测构成了评测体系的大部分内容。

![640 (5).jpeg](Scenes%20Weekly%20%2315.assets/640%20(5).jpeg)

你可以看到用户满意度调查方面和平时所作的产品用户体验调研并无过多区别。总分 100 分，60 分以上即为合格，合格后会被授予信息无障碍标识，如下图。

![640.jpeg](Scenes%20Weekly%20%2315.assets/640.jpeg)

在评测体系提到的「设计规范」中，还可以看到很多具体的规定，比如最小字号不得小于 18 dp/pt，段落内行间距至少为 1.3（在 **GB/T 37668-2019** 中三级最高标准为 1.5，实际上正文一般采用 1.7 左右），4.5:1 的对比度，触摸区域尺寸（和HIG、MD几乎一样）等规定。简单总结就是平时多加注重 a11y 在此评测体系里便不会遇到什么问题——当然事实上不同的产品在不同的场景下，要做的远比说的复杂。

设计规范与评测体系出处（工信部）↓

[工业和信息化部办公厅关于进一步抓好互联网应用适老化及无障碍改造专项行动实施工作的通知](https://www.miit.gov.cn/zwgk/zcwj/wjfb/txy/art/2021/art_b04e1baa455c448b80fb790d7c50bfd4.html)

GB/T 37668-2019 文件 ↓

[国家标准](http://www.gb688.cn/bzgk/gb/newGbInfo?hcno=35ECC696805C1A67C93B74FB6D)

---

# **周一**

iOS 15 Beta 3 一项改进是，**Safari** 的地址栏下移到和键盘融合在一起（左一）。之前是常驻在顶部，这样改动可以在输入时更加节省精力不用上下移动目光。

![640 (1).jpeg](Scenes%20Weekly%20%2315.assets/640%20(1).jpeg)

并且地址栏优化了输入时建议字段，更加方便（左二）。

长按地址栏也可以直接选择刷新，不用点三个点菜单（右一）。适用于滑到了页面底部时，无法触发在网页顶部的刷新机制。

---

# **周二**

**Apple Style Guide** 是苹果品牌的文案写作指南，涉及到设计介绍、文档到用户界面各种领域，目的是使品牌对外发声一致。

![640 (2).jpeg](Scenes%20Weekly%20%2315.assets/640%20(2).jpeg)

这份指南在今年六月份有所更新。虽然原文是英语但也有一定通用性。比如指南告诉你不要把 Airdrop 用作动词：

> 错误 你可以隔空投送照片和文档给附近的其他设备。

> 正确 你可以使用隔空投送将照片和文档传给附近的其他设备。

以及指导你何时称之为图标，几时称之为按钮（如下图）这种界面控件的描述歧义问题。当然对控件的解释不会面面俱到，详情还是要去看 HIG。

![640 (3).jpeg](Scenes%20Weekly%20%2315.assets/640%20(3).jpeg)

谨慎的苹果也没有忘记包容性写作指导，比如注意措辞（某个单词结合上下文后可能会有歧义），避免使用暴力、压迫性词语（不能说 kill 进程，不要用 master 之类）、避免俗语谚语成语、避免通过颜色表达除颜色以外的概念（不能说黑名单，只能说白底黑字）、能用 they 就不用 he or she（这个中文怎么办）等。

剩下还有一些单位进制、技术文档、国际化的少部分信息。

地址 ↓

[https://help.apple.com/applestyleguide/#/](https://help.apple.com/applestyleguide/#/)

---

# **周三**

专门为桌面端设备 Twitter 浏览体验打造的 **Tweet Deck** 时隔近20个月得到更新。保留了之前的多列浏览模式，在旧版的各种奇怪交互上做了优化。

![640 (4).jpeg](Scenes%20Weekly%20%2315.assets/640%20(4).jpeg)

我之前把 List 删了好多，所以用起来并无太多体验提升。UI 上也比较简陋，不如 iPad 上的 Aviary。

目前官方说正在灰度测试中，不过你可以在浏览器 Console 里输入 *document.cookie="tweetdeck_version=beta"* 开启测试。

体验 ↓

[X Pro](https://tweetdeck.twitter.com/)

---

# **周四**

专门搜集各种移动端 app 界面的 **mobbin.design** 迎来了改版。距离他们上次发布问卷调查已经很长一段时间了。

网站的 UI 整体更新，加入了 Android 应用的截图（原本只有 iOS），整合了分类和搜索（没有之前那么直观，但加入了 OCR 搜索），可以选择查看旧版本应用截图（需要付费会员）。

![640 (6).jpeg](Scenes%20Weekly%20%2315.assets/640%20(6).jpeg)

免费用户依然不会受到太多影响，而且连 OCR 搜索都对所有人开放了权限。看 About 说团队已经有人全职做这个事了，希望越做越好吧，别像隔壁 uisources 一样沉默已久。

---

# **周五**

**a11y** 不断得到重视，隔一阵子就会出现一些信息、资源。

![640 (7).jpeg](Scenes%20Weekly%20%2315.assets/640%20(7).jpeg)

The A11Y Project ↓

[Checklist - The A11Y Project](https://www.a11yproject.com/checklist/)

Access Guide ↓

[Homepage - Access Guide](https://accessguide.io/)

Geri Reid’s WCAG for Designers ↓

[Geri Reid - WCAG Accessibility Checklist](https://gerireid.com/wcag-for-designers.html)

---

# **杂事**

1、我其实很久没有看 Morning Brew 了，然后上周末发现他们不知道什么时候开了个 **Sunday Edition**，内容更轻松、简洁，没那么商业化，排版也「欢快」了不少，这种更适合我的口味。往前翻了一下，原来 4 月 4 日就开通了第一期。

![640.png](Scenes%20Weekly%20%2315.assets/640.png)

---

2、上周的 weekly 提到了苹果对于**居家办公**的态度问题，现在该返工政策已经从九月推迟到十月。

来源 ↓

[Apple Will Delay Bringing Employees Back to Offices Until at Least October](https://www.macrumors.com/2021/07/20/apple-delays-return-to-offices/)

---

3、Twitter 在灰度测试评论 **up/down vote** 功能，又一次引发了争议。尽管官方一再声明这仅是一项调研；这不是「不喜欢」（dislike）按钮；downvotes 仅自己可见；不会影响评论回复的排序。但群众依然对这个功能的未来产生担忧，很多人认为既然不喜欢的内容一般都会自动忽视，现在非要让我和内容产生交互，是不是居心叵测？

一旁隔岸观火的 Reddit 看热闹不嫌事大：

![640 (1).png](Scenes%20Weekly%20%2315.assets/640%20(1).png)

不难理解为什么大家都对 downvotes 存疑，我在 2019 年写过一篇 DesignNews 社区如何走向没落的文章里提到过， downvotes 可能反而会减少互动。而目前看来 Twitter 只是想把那个图形做为发泄口径，本身无任何意义。

查看 Designer News 的没落 ↓

[EVA 02](https://fenx.work/Designer-News-48c8253f501d4ca4b78e9de8f4854608)

我的感受是，这项改动还不好去轻易的下结论。但近一年里 Twitter 的迭代动作明显增加，传统 SNS 巨头确实感受到了新兴媒介的压力。

查看原推 ↓

[登录 Twitter，关注Twitter Support](https://twitter.com/TwitterSupport/status/1417920469265788931)

---

4、Fast Comany 列举了 **2021 年最具生产力的 26 款应用**，很多都不陌生，一些 app 在之前的 weekly 里也提到过。

查看原文 ↓

[https://www.fastcompany.com/90652944/best-productivity-apps-2021](https://www.fastcompany.com/90652944/best-productivity-apps-2021)

---

5、Daryl Ginn 建了一个网站叫 **Godly Website**，搜集了一些 "godlike" 网站，质量确实很不错。现在已经搜集 100 多个网站了。

网站 ↓

[Godly — The Best Web Design Inspiration](https://godly.website/)

---

6、老图：**Airpods** 带来的收入在各大科技公司中的对比。

![640 (2).png](Scenes%20Weekly%20%2315.assets/640%20(2).png)

Twitter @gannonbreslin

---

7、劳模 rogie 最近暗示 Figma（通过插件）即将支持苹果的 **HEIC** 格式导入。

![640 (3).png](Scenes%20Weekly%20%2315.assets/640%20(3).png)

Figma 的社区力量太强大了（虽然他应该算半个官方人员）。另外支持 gif 导入，是不是意味着实况照片也能……？

另外 Figma 最近也对 pencil 功能和半透明图层阴影效果显示做了优化，还有其他一些小功能详见 Figma Releases ↓

[Figma Releases](https://releases.figma.com/)

---

8、Kieran Healy（@kjhealy）分享了一张麦金塔的古早**说明书**：

![640 (4).png](Scenes%20Weekly%20%2315.assets/640%20(4).png)

什么叫界面直观？顺着直觉就是直观。

评论区还有人挖出了 1984 年 **Macintosh Guided Tour** 中的鼠标教程示例：拖动鼠标，让老鼠吃到奶酪。

![640 (5).png](Scenes%20Weekly%20%2315.assets/640%20(5).png)

这些想法我们现在已经感受不到了。

视频地址 ↓

[Macintosh Guided Tour (Part 1/7): Intro & "Mousing Around"](https://www.youtube.com/watch?v=1pwammW5syw)

---

9、这一周 Brand New 社区对 **Piedmont Art Walk** 的新标识赞赏不已。

![640 (6).png](Scenes%20Weekly%20%2315.assets/640%20(6).png)

Piedmont Art Walk 是 Piedmont（加州）本地一项艺术展览活动，由非营利组织 Piedmont Arts Fund 举办。每年春季的这个时候，当地的数十位艺术家就会搬出自己的艺术品，募集到的资金用于本地艺术教育事业的发展。

可以看到，旧版的标识非常糟糕，主次不明显，字体搭配更是灾难级。新的标识请了 Mucho 重新设计，真的让 ART 走起来了——

![AnimatedImage.gif](Scenes%20Weekly%20%2315.assets/AnimatedImage.gif)

它的标识延展所展现的灵活与趣味性，更是让人印象深刻。多说无益，还是自己感受下 ↓

[Walks like a Charm](https://www.underconsideration.com/brandnew/archives/new_logo_and_identity_for_piedmont_art_walk_by_mucho.php)

[Piedmont Art Walk | Mucho](https://wearemucho.com/project/piedmont-art-walk/)

---

10、我已经想不起来多久没有用到像 **Honk** 一样有趣，流畅，无干扰的 app 了—— Honk 是一个实时交流的社交 app，最大的特点是两个人聊天不会像是传统的 log 形式一样，而是能看到对方的打字成句过程。

![640 (7).png](Scenes%20Weekly%20%2315.assets/640%20(7).png)

最令人吃惊的是 app 的整体流畅度——直接惊掉我的下巴——到底是怎么做到如此流畅的，太舒服了（iOS15 beta3）。这就是 native app 的魅力吗？

[Honk](https://honk.me/)

---

11、那些数十亿估值的大公司初创时的 Pitch Deck 是怎样的，有人就做了这么一个网站去展示这些：**Billion Dollar Pitch Decks**。

用来观察这些公司怎么去讲清楚自己业务上的长处。资源并不是独家的，所以只是个搜集整理而已 ↓

[Startup Pitch Decks | Billion Dollar Pitch Decks](https://www.billiondollarpitchdecks.com/)

---

12、有团队创作了 50+ 个免费 AI 驱动的小工具，比如歌词生成、AI 做梦、游戏创意生成等等。很有趣。

![640 (8).png](Scenes%20Weekly%20%2315.assets/640%20(8).png)

链接 ↓

[BoredHumans.com - Fun AI Programs You Can Use Online](https://boredhumans.com/)

---

13、今年的**奥杜邦摄影奖**（Audubon Photography Awards）已出炉。闲暇时间可以欣赏一下鸟类百态。

![640 (9).png](Scenes%20Weekly%20%2315.assets/640%20(9).png)

Grand Prize: Carolina Fraser

顺便一提我最喜欢这张的调色与焦距（虽然我并不喜欢加拿大鹅）：

![640 (10).png](Scenes%20Weekly%20%2315.assets/640%20(10).png)

地址 ↓

[The 2021 Audubon Photography Awards: Winners and Honorable Mentions](https://www.audubon.org/magazine/summer-2021/the-2021-audubon-photography-awards-winners-and)

---

**14、PaintUp** 可以把平面笔画转变为 3D 的形状 ↓

[PaintUp](https://technohippy.github.io/teddyjs/)

---

15、Jordan Nelson（@JordanTeslaTech）吐槽**特斯拉**会把月亮识别成黄灯……

![640 (11).png](Scenes%20Weekly%20%2315.assets/640%20(11).png)

其他情况比如有些特殊地方的指示灯停在中间是红灯，特斯拉依然会识别为黄灯，真的色盲。「没事，是 Edge Case。」

---

16、东京奥运会也在本周开幕，开幕那天的 **Google Doodle** 相当惊人。一段日本动画开场过后，是 GBC 风格的七个小游戏。体量也太大了。

![640 (12).png](Scenes%20Weekly%20%2315.assets/640%20(12).png)

顺便一提动作制作是 **STUDIO 4°C**，你可以在归档页看到其背后的故事 ↓

[Doodle 冠军岛运动会开始啦！](https://www.google.com/doodles/doodle-champion-island-games-begin)

如果你的 Chrome 升级到最新的 92，小恐龙游戏还会变成奥运主题，只需在流程中触碰到蓝色的「圣火」即可变换各种运动场景，有时玩法也会略微改变。下图为游泳和跨栏。

![640 (14).png](Scenes%20Weekly%20%2315.assets/640%20(14).png)

![640 (13).png](Scenes%20Weekly%20%2315.assets/640%20(13).png)

刷新 chrome://dino/ 即可更换运动项目。

---

17、前天（22号），**Clubhouse** 对公众开放。

![640 (15).png](Scenes%20Weekly%20%2315.assets/640%20(15).png)

详见博客 ↓

[Clubhouse Opens Wide: Invites No Longer Required 🎉](https://blog.clubhouse.com/opening-day/)

我更在意他们每月一换的 app icon。

![640 (16).png](Scenes%20Weekly%20%2315.assets/640%20(16).png)

---

**18、Mapbox Studio** 能让你像 Ps 一样去定制各种地图样式。

![640 (17).png](Scenes%20Weekly%20%2315.assets/640%20(17).png)

对我来说很新颖，国内有类似做定制的产品吗？

---

19. 斗鱼发布了自己的品牌字体，**斗鱼追光体** ↓

[斗鱼追光体](https://www.douyu.com/topic/douyuZGT)

但是在我的 mac 上显示 name 表有问题……修复了下才能用。

![640 (18).png](Scenes%20Weekly%20%2315.assets/640%20(18).png)

---

20、之前 GPT-3 刚出来时不是有人做了个 AI 帮设计 UI 的插件吗？现在有人想正经开发这个项目了，**Tricycle**。

![640 (19).png](Scenes%20Weekly%20%2315.assets/640%20(19).png)

等待颠覆 ↓

[https://tricycle.ai/](https://tricycle.ai/)

---

21. meme 一则：

![640 (20).png](Scenes%20Weekly%20%2315.assets/640%20(20).png)

Rahul Chakraborty（@hckmstrrahul）

---

封面使用了 Fontworks 的 RocknRoll One 字体。