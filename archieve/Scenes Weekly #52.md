# Scenes Weekly #52

2022-05-02

\> 设计视角下的世界——

第 51 期请[在此查看](./Scenes Weekly #51.md)。

本期出现：

- Figma 桌面端更新
- 在线阅读的最佳字体特性调查
- GT Planar 字体发布
- macOS 菜单栏图标规范
- Elon Musk & Twitter | Final Season
- DALL.E 2 与设计奇点思考
- GPT-3 赋能微波炉
- 其他：Oldest Search、Steam Deck 锁屏界面吐槽、Wikipedia A/B Test、渐开线齿轮动画生成器、 Linear Features、Hock Wah Yeo 的游戏包装设计、抵制 Google AMP、浏览器诗歌、Earth Reviews、Felix 教你赛博化、ProtoPie 付费计划更新、Meco 推出网页版、另类的 GitHub Store

如有格式异常建议点击最上方「在浏览器中访问」。

---

劳动节快乐，今天也是不用生产价值的一天。

感谢 [DEX 周刊](https://newsletter.dex.group/) 上期的友链推荐。之前总觉得在肯德基里吃麦当劳不太好，不过既然肯德基开了外带专区，决定带着汉堡王进去试吃一下。

---

# 摘录

这周看过的一些——

> The idea and service is all that matters to me, and I will do whatever it takes to protect both. Twitter as a company has always been my sole issue and my biggest regret. It has been owned by Wall Street and the ad model. Taking it back from Wall Street is the correct first step.

—— Jack Dorsey - [摘自](https://twitter.com/jack/status/1518772754782187520)

---

# 杂事

1、Figma 上个月 27 日更新了桌面端应用——

- 标签也显示 favicon 了，并且可以自定义（emoji + 空格 + 文件名）；
- 鼠标经过可以显示全部文件名；
- Reload Tab 上加了个 Pin Tab 固定标签；
- 右上方 ··· 可以访问最近关闭的文件；
- 标签栏可以拖动建立新窗口；

总之一切更贴近浏览器标签的使用习惯。

![388be2b570ca46f298c7366dba93eca9.png](Scenes%20Weekly%20%2352.assets/388be2b570ca46f298c7366dba93eca9.png)

{上图：Figma 114.2.1 版本中标签栏改动}

→ Release Notes

[Figma Releases: 🖥️ Desktop app tab updates](https://releases.figma.com/2022/04/desktop-app-tab-updates.html)

---

2、Nielsen Norman Group 分析了 Adobe 的一篇阅读速度研究报告，该报告试图找出在线阅读的最佳字体特性，但结论是——没有。

- 使用的实验字体为 Times、Helvetica、EB Garamond、Noto Sans、Arial 等耳熟能详的几位；
- 测试的三种文本显示方式：通知或可穿戴设备上的小字单词、短篇以及长篇阅读；
- 实验的三个指标：主观偏好字体、每分钟阅读词数（WPM）和理解分数（读完内容后回答问题）；
- 每个用户只测试 5 个字体；

![5b218271f9f44ee4aac7c9a82aad0063.jpeg](Scenes%20Weekly%20%2352.assets/5b218271f9f44ee4aac7c9a82aad0063.jpeg)

{上图：阅读速度各项测试结果}

结果为 Garamond 平均阅读速度最快，312WPM。Open Sans 最慢，254WPM。两者相差 23%。但这是总体平均的效果，要论每个人五个字体中阅读最快的那个字体，是 Franklin Gothic （59%），Garamond 为 48%。但 Franklin Gothic 只有 271WPM，这些其妙的差异和实验对象的个体阅读能力有关系，擅长阅读的人在看 Garamond 字体内容时如虎添翼，但对平时不怎么阅读的人就不那么奏效。

在偏好字体选择上，很多人不知道自己喜欢哪个字体（太真实了），并保持默认字体设置。就算设置其他字体一般也没有逻辑，有的人甚至会选择等宽字体。

年龄也会影响阅读速度，实验结果表明 50 岁的用户比起 30 岁需要花费更多的时间（11%）完成阅读。Garamond、Montserrat 和 Poynter Gothic 更适合年老的实验对象。

> The takeaway is that, if your designers are younger than 35 years but many of your users are older than 35, then you can’t expect that the fonts that are the best for the designers will also be best for the users.

所以啊，之后劳动力没那么密集后，老年设计师去做老年适配设计，年轻设计师就去做年轻向的设计，别 35 岁就直接把人劝退了（？）

→ 原文

[Best Font for Online Reading: No Single Answer](https://www.nngroup.com/articles/best-font-for-online-reading/)

---

3、Oldest Search 是一个古怪的搜索入口，它从 Google 搜索中调用时间正序的搜索结果，优先显示最久远的内容。这样搜索相关性就会差很多，比如搜索 UI design 在第一页会出现 2001 年的 Ant Design 官网…… 但冲浪时就需要这种新奇的东西来调剂口味 :)

→ 网站

[Oldest Search - Search for the oldest result on internet.](https://www.oldestsearch.com/)

---

4、对于 Steam Deck 这样的用户友好型产品，我总是想不遗余力地去广而告之。上周 Valve 又更新了 SteamOS，添加了锁屏、成就、本地化键盘、多窗口切换、以及 fTPM 支持（可以刷 Windows11 了）等等特性。其中锁屏界面我有些眼熟——

![48ec3581543246d1a2c52d93228fa159.jpeg](Scenes%20Weekly%20%2352.assets/48ec3581543246d1a2c52d93228fa159.jpeg)

{上图：SteamOS 更新后的锁屏界面}

我在前年有[吐槽过](https://weibo.com/6728914621/JtyZheGlf) Xbox Passkey 界面就是这个锁屏键位，不知道是如何决策这个键位映射的。

![74edb6dea07f4a409be14296ffe632e5.png](Scenes%20Weekly%20%2352.assets/74edb6dea07f4a409be14296ffe632e5.png)

{上图：Xbox Passkey 键位的原图和个人修改版}

我的修改基于以前使用的九宫格实体键盘体验。在一些 S40/S60 游戏中，2468 会当成方向键，1379 会被当成类似肩键和扳机的键位，于是便逆向映射一下。没想到 SteamOS 直接把作业抄过来了…… 想知道谁是这个交互的始作俑者。

→ 其他更新详情

[Steam :: Steam Deck :: 锁屏界面更新](https://steamcommunity.com/games/1675200/announcements/detail/3216142491800836086)

---

5、看到 Grilli Type 新字体发布后，第一反应是他们又做了什么神仙网站。这次发布了 GT Planar，主要特色是探索了字体在 -45° 和 +45° 极限倾斜程度情况下的形变张力——欢迎来到瑞士未来主义。

![85776727f9374378a3be5e745e6191af.gif](Scenes%20Weekly%20%2352.assets/85776727f9374378a3be5e745e6191af.gif)

{上图：GT Planar 中直角曲线特性}

GT Planar 带有明显的机械感，以往笔画的尾部和连通处都做了平直的处理，以减少极限倾斜后不和谐角度，同时符合大众对于科幻风味的认知，比如 NASA 的蠕虫标识。小写字母 r u n 的字棱处在倾斜时还会保持一定的垂直角度，大写字母提高了重心。总之，正常情况下可以视作一款带有 STRAIGHT ALTERNATES 属性的字体，想用上那夸张的倾斜比例并不容易。

当然这次的主角应该还是网站本身，试用字体的那个 HUD 绝了。

→ 网站

[One moment, please...](https://gt-planar.com/)

---

6、给 macOS 产品设计菜单栏图标不是常有的事，Apple HIG 中也没提到详细的参数说明。高产的 Marc Edwards 做了一些总结：

- Mac 的菜单栏高度从 System 1 的 19pt 开始，到现在 Monterey 已增加到 24pt；
- 如果是最新带「刘海」的 macbook，默认缩放下高度会变为 37pt；
- 但实际内容区域高度为固定的 22pt，建议图标在 16x16 区域绘制；

![ac73d464b23a40e0bb5e31a0953c6d8b.png](Scenes%20Weekly%20%2352.assets/ac73d464b23a40e0bb5e31a0953c6d8b.png)

{上图：菜单栏图标区域结构}

- macOS 会无视颜色，只保留 alpha 通道信息；
- 格式支持 SVG、PDF 或 PNG，也支持代码去实现动态信息；

→ 原文

[Designing macOS menu bar extras](https://bjango.com/articles/designingmenubarextras/)

---

7、Wikipedia 设计团队分享了以简单的 A/B Test 为出发点，派生上一级流程的变体测试，以优化编辑者体验，促进编辑欲望的流程。配图比较糟糕，不多说什么了……

→ Designing variant experiments is as simple as A/B. See?

[Designing variant experiments is as simple as A/B. See?](https://design.wikimedia.org/blog/2022/04/04/designing-variant-experiments.html)

---

8、Gear Generator 是一个生成多个渐开线齿轮啮合的小工具，输入参数后便以实时动画的形式展示机械美感，能导出 SVG 和 DXF，甚至可以用做设计资源。注意原网站 Chrome 无法渲染 AVG，开发者推荐使用 Opera 或 Firefox。

![c77ca7f02f2149f18685fb4a0a9021f8.png](Scenes%20Weekly%20%2352.assets/c77ca7f02f2149f18685fb4a0a9021f8.png)

{上图：齿轮在蓝图纸背景上生成并运转}

→ 网站

[Involute spur gear generator and simulator](https://geargenerator.com/)

---

# 小事

**[Twitter](https://designscenes.zhubai.love/posts/2130213690493816832#:~:text=%E5%B0%8F%E4%BA%8B-,%E3%80%8ATwitter%20%26%20Musk%E3%80%8B,-%E6%9B%B4%E6%96%B0%EF%BC%9A) 更新：**

这里是 Elon Musk & Twitter 年度大剧第三季，貌似也是最终季。大家基本都已经知道 Twitter 已是 Musk 的囊中之物，这其中还有几点：

- 这场交易可能将会持续半年，但也说不准上周四应该是 Twitter 最后一次财报披露了；
- 毒丸计划没实施，更像是一个对 Musk 现金流「试探」；
- 很多人转移到 Mastodon，包括[欧盟委员会](https://twitter.com/EU_Commission/status/1519639071823380481)。长毛象官方也发布了一篇文章 [Twitter buyout puts Mastodon into spotlight](https://blog.joinmastodon.org/2022/04/twitter-buyout-puts-mastodon-into-spotlight/)；

![6c38808596254c8daae46a9c23983a99.png](Scenes%20Weekly%20%2352.assets/6c38808596254c8daae46a9c23983a99.png)

{上图：Mastodon 标识}

- Tesla 的股票涨跌是 125 亿美元贷款中很大风险因素；
- 监管阻拦的可能性比较小，涉及股东利益，同时不构成理论上的反垄断；
- 之后谁来做 Twitter CEO？管理层甚至员工层大清洗？
- 由于杠杆收购的特性，Twitter 的盈利问题也牵扯到 Musk 之后的还本付息…… 首富哥云淡风轻说了不关心，实际还是得上点心；
- Musk 这时候还不忘[嘲讽 Twitter 高管](https://twitter.com/elonmusk/status/1519377424437243904) Vijaya Gadde（首席法律官），导致后者成为「网暴」对象。虽然在协议中有提到 Musk 不能在这个期间诋毁 Twitter，但显然 Twitter 也不会追究…… 他给的太多了；
- Musk 提到他说的自由言论是合法（遵守当地法律）的前提下，可 Musk 自己的[黑历史](https://news.ycombinator.com/item?id=31162721)就太多了。而且在 Twitter [现有的规则](https://help.twitter.com/en/rules-and-policies/twitter-rules)之中，一些虚假的选举 / 医疗信息、垃圾邮件、暴力、自残等内容是被列为不合规的，但是按照 Musk 的说法这些又（在某些地区）「并不明确」是违法的。欧盟罚单警告. jpg



**DALL.E 2 更新：**

[第 50 期](https://designscenes.zhubai.love/posts/2127677128824475648#:~:text=1%E3%80%81%E4%B8%8A%E5%91%A8%20OpenAI%20%E7%9A%84-,DALL.E%202,-%E7%88%86%E7%81%AB%E5%90%8E)谈到了 DALL.E 2 过于强大的能力背后所潜藏的风险，Nathan Baschez 提供了另一个讨论角度，大意是在 2015 年左右，之前的网站经常使用现实取景图片去做 UI 一些表达，之后的网站开始把这些替代为富有「设计感」的插画风格。Baschez 认为这或许与 Unsplash 等无版权图库网站的兴起有关，无需支付费用就可以立即获得精美的合规图像大大降低了设计的表达门槛，与此对比，融合了各种艺术风格的人工定制插画显得更「稀有且昂贵」。联想到现在更加流行的 3D 风格，对同等水平的插画来说也是一种「上位替代」，有着新鲜的抽象图形和额外的门槛，趋势在差异化的道路上不断前进。

DALL.E 2 的到来可能又会像 Unsplash 一样改变这一趋势，几句话生成符合需求的图像，自己再小修改一下就可以直接使用，实现了「众图平等」。

![cc2885f4a892489d8da5cebfb32f5f6f.png](Scenes%20Weekly%20%2352.assets/cc2885f4a892489d8da5cebfb32f5f6f.png)

{上图：炉石传说卡牌生而平等的 meme}

当到达这一「设计奇点」时，差异化竞争开始转换到与现有训练数据的对抗。以历史的角度来看更像是文艺复兴前期的感觉，类似抵制 AI 神权云云。很有趣的思维实验，实际上 DALL.E 2 能像现在 GitHub Copilot 一样做好辅助功能就心满意足了。

→ 原文

[DALL·E 2 and The Origin of Vibe Shifts](https://every.to/divinations/dall-e-2-and-the-origin-of-vibe-shifts)

顺便一提已经有个开源版的 [DALL·E mini](https://huggingface.co/spaces/dalle-mini/dalle-mini)，可以试玩一下（虽然与本体有不少的差距）。

![82cdd15c90c842948b2c0252b2248f14.png](Scenes%20Weekly%20%2352.assets/82cdd15c90c842948b2c0252b2248f14.png)

{上图：使用 DALL·E mini 生成 "a blue design newsletter on the table" 图像}

---

1、Linear 这款产品很多人应该都熟悉了。最近他们上线了 /feature 页面，用于全方位介绍产品功能。依然是很舒服的深色模式，值得注意的是 hover 效果加入了类似 Fluent Design 光照效果。目前该效果已经在 Windows11 上看不到了。

→ Linear Features

[https://linear.app/features](https://linear.app/features)

---

2、Hock Wah Yeo 设计的上世纪游戏包装为了契合游戏风格，大都不规则而具有鲜明特色，但成本较高，运输和摆放不便等因素，逐渐淡出大众视野。 It's Nice That 这篇文章带你回顾了 Yeo 的包装设计鉴赏。

→ Outside the box

[Outside the box: the mind-boggling video game packaging of designer Hock Wah Yeo](https://www.itsnicethat.com/features/hock-wah-yeo-game-packaging-graphic-design-260422)

---

3、Lucas Rizzotto 的童年有着一个幻想中的朋友，是他们家厨房的微波炉，名字叫 Magnetron。Rizzotto 为这位微波炉兄弟塑造了完整的人物背景设定，英国绅士、一战老兵、流浪诗人等等，荒谬又真实。为了复活 Magnetron，Rizzotto 在 Amazon 买了一台智能微波炉，接上麦克风和扬声器，配置好 GPT-3 与机器的 API，实现交谈的方式控制微波炉，仿佛外接了新大脑。

如何让这个「素体」成为 Magnetron 呢？Rizzotto 写了一本 100 页的文档，里面都是 Magnetron 的详尽生活记录，然后告诉 GPT-3 这些都是真实的。接下来测试的大部分对话都比较顺利，Rizzotto 在文档里面写下了只有 Magnetron 知道的童年往事，偶尔在对话中提到还会感到一些惊喜。但是，偶尔的几次回复中，Magnetron 表现出了极端的暴力。

![44dd8662f89d48ed801e8aa201583943.jpeg](Scenes%20Weekly%20%2352.assets/44dd8662f89d48ed801e8aa201583943.jpeg)

{上图：Magnetron 突然的杀意}

Rizzotto 想起自己在编写背景时有写到 Magnetron 在一战的记忆，那场战争里他失去了家庭。这是制造了一种 AI PTSD 吗？Magnetron 甚至对 Rizzotto 说要他进入微波炉内，Rizzotto 假装进去，下一刻微波炉自己启动了，很明显是有了杀心。询问原因，Magnetron 回答道 "Because I wanted to hurt you the same you hurt me"。最后 Rizzotto 关闭了电源，将微波炉肉体请出了家门。

去年还有个给 Clippy 注入灵魂的[视频](https://www.youtube.com/watch?v=ATWV3bPvoDg)，无论真假（实际 GPT-3 的输入成本并没有那么轻描淡写，价格也不菲），视频本身还是挺好看的。上述内容来自[该 Twitter Threads](https://twitter.com/_LucasRizzotto/status/1516205625662836739)。

→ 还有个视频版

[I gave my microwave a soul with AI and it tried to kill me](https://www.youtube.com/watch?v=C1G5b_2PYj0)

---

4、最近几期搜索引擎的信息莫名有点多。Brave 之前表示，他们将推出 De-AMP 这个功能，帮助用户跳过 AMP 页面，直接访问原网页。DuckDuckGo 随后跟进这一举措，两者都对认为 AMP 是 Google 在鼓励网站发布商使用更多的 Google 服务和广告标准，进一步巩固自己的垄断地位。Google 搜索公关回应称 AMP 并不影响网页排名。

这不是一个新鲜的事实，AMP 被嫌弃已久（Wordpress 反而一直在强调 AMP 指标），Twitter 早就重定向到网页，一些插件也能实现类似功能。

国内的话，「百度版的 AMP」MIP 去年就下线了，在那之前就大举宣发熊掌号，包括有着现金激励的百家号等等让你直接无法溯回原内容网页，只留下一个品牌展示。高。

→ 原文

[https://thenextweb.com/news/duckduckgo-and-brave-anti-amp-features](https://thenextweb.com/news/duckduckgo-and-brave-anti-amp-features)

---

5、iframe 是我们常见的一种网页元素，用于在当前文档嵌入另一个 HTML 文档。Anonymous Animal 利用这项略微过时的内联框架，和文字结合起来，形成了一首 15 分钟的浏览器在线诗歌！

该项目被收录在 [the html review](https://thehtml.review/) 今年第一期里。The html review 是一份以网络为媒介的实验文学期刊。

→ 可能需要放置几分钟

[Anonymous Animal](https://anonymous-animal.neocities.org/)

---

6、Neal Agarwal 在他的 Neal.fun 上做了很多有趣的小工具，[第 36 期](https://designscenes.zhubai.love/posts/2087096655987212288#:~:text=12%E3%80%81-,Neal.fun,-%E6%98%AF%20Neal%20Agarwal)提到过他做的石头叠叠乐。最新的是一个叫做 Earth Reviews 的点评平台。不同的是，这次是来点评身边最常见的事物，比如打嗝有 3154 人评论，仅获得 1.4 分，满分 5 分。结婚获得了 3 分（1631 人评分），猫猫获得了 4.4 分（4194 人评分）。评分最高的是电子游戏，4.8 分，5588 人评分。谁会不喜欢游戏呢？

![0b246c210d774495bfc636592ed55b7b.png](Scenes%20Weekly%20%2352.assets/0b246c210d774495bfc636592ed55b7b.png)

{上图：Video Games 评价界面}

→ 网站

[Earth Reviews](https://neal.fun/earth-reviews/)

---

7、Felix Krause 在过去三年里跟踪关于自己的 100 多种不同类型数据，收集了超过 38 万个数据点。他想搞清楚睡眠、季节、天气、工作等因素是怎样影响他的生活的。作为赛博化的第一步，Krause 搭建了一个网页来展示他每天的位置、心情、食物能量摄取、身体状况等数据。极为详尽，其中有很多要手动输入的数据，比如他自己开发了个 bot 每天问他 4 次心情如何，0-5 的李克特量表。太佩服了。

→ How is Felix today

[https://howisfelix.today/](https://howisfelix.today/)

---

### 8、几个产品更新——

8.1、一直以来，ProtoPie 的高价位姿态与其想打造的亲民人设相矛盾，它确实是一款强大的原型应用，但是 30 天试用后订阅付费，没有照顾到低频使用者。上次接触 ProtoPie 时就感到奇怪，明明是一款有着足够深度的原型工具，却总是打着易上手门槛低去吸引用户。要易上手的话为什么不去用 Figma 自带的 Prototype 呢？好，你有更强大的表达式和变量，然后 30 天里，去掉正式工作时间，等上手了发现也该付费了，付费后发现使用频率有没那么高…… 食之无味，弃之可惜。

五年后，ProtoPie 似乎想通了。上个月 28 日官方发文称将会更改付费计划，变为有原型限制的免费使用计划，和无限制的付费订阅计划。5 月 30 日生效。

→ 详见

[Introducing the New Free & Pro Plans](https://www.protopie.io/blog/introducing-the-new-free-pro-plans)



8.2、[Meco](https://www.meco.app/) 是一款优化整理 newsletters 专用的收件箱，之前用过，自动识别和转移订阅都很方便，因为只有 iOS 端无法在 mac 上查看便弃之。[第 13 期](https://mp.weixin.qq.com/s/Q37AwaEC9ZtPXEwAM1ypvQ#:~:text=%E4%BA%86%20Big%20Mail%20%E5%92%8C-,Meco,-%E4%B8%A4%E4%B8%AA%20inbox)有对比过它和 Big Mail 的差别。现在 Meco 推出了网页版，该考虑要不要用回来🤔。

→ 网页版

[Meco](https://web.meco.app/get-started)



8.3、GitHub Store——注意不是那个官方卖周边的地方——是一个第三方的买卖 repository 的网站。开发者一边肆无忌惮地使用了 GitHub 这一注册商标混淆视听，一边在做着很搞笑的事情，看来每个人对开源的看法有很大的不同。

→ 围观

[https://githubstore.net/](https://githubstore.net/)

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

---

# 劳逸

![31a90b36024948b3a4193852d2353b8a.png](Scenes%20Weekly%20%2352.assets/31a90b36024948b3a4193852d2353b8a.png)

{上图：SAMURAI BRINGER Banner}

中文名叫侍神大乱战，一款和风无双 Roguelite 游戏。你是须佐之男，老婆奇稻田姬被八岐大蛇带走，你要借助战国猛将的力量去夺回自己的幸福。特色的玩法在于你可没有天羽羽斩，全靠自己组合不同的武器动作模组和被动技能去弑敌。流程中箭插入的解谜小游戏是个断节奏的败笔。

→ 游戏获取

[Steam 上的 侍神大乱战](https://store.steampowered.com/app/1851280/_/)

---

# 映像

现实拟像放映——

![f5a95ae64492427190a14398cfdc1e32.jpeg](Scenes%20Weekly%20%2352.assets/f5a95ae64492427190a14398cfdc1e32.jpeg)

上图：Mother as a Mountain (Black)

© Anish Kapoor

---

# 温故

→ [Scenes Weekly#3](./Scenes Weekly #3.md)

- HN 的重设计：Box Piper Hacker News
- 糟糕交互收集：Grumpy Website
- UX 术语词典：UX Lexicon
- Grilli Type 发布了 GT Maru 字体（巧了）
- Twitter 推文菜单排序细节
- 微信设计团队《设计 watchOS App》
- ATypI 宣布撤回 Vox 字体分类法

---

喜欢本文的话，欢迎分享、订阅。

第 51 期请[在此查看。](./Scenes Weekly #51.md)

本次封面使用了 Plus Jakarta Sans 字体。

