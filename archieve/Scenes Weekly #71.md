# Scenes Weekly #71

2022-09-24

\> 设计视角下的世界——

第 70 期请[在此查看](./Scenes Weekly #70.md)。

本期出现：

- iOS 16.1 电量百分比更新（二）
- 公众科学中的排队设计
- 重读HIG（十一）- Launching
- 平均寿命与预期寿命区别
- Platformer 第二年总结
- YouTube 的「不感兴趣」没什么用
- 其他：Snapchat 复杂好处、老照片上色的网页应用 Colorize Pictures、Peloton 商业模式、Canva Docs 推出、iFixit 拆解 iPhone 14、Morgan Stanley 3500万美元罚款、游戏驴子成立自己的游戏发行

如有格式异常建议点击最上方「在浏览器中访问」。

---

最近到市集出摊了几次。为了将顾客往线上引流，我们决定扫码就送冰箱贴（低获客成本）。扫的码是小红书和抖音，任一关注都可以。在观察了 60 多名顾客扫码行为后，想对小红书说两个消息：

- 好消息：大多顾客使用小红书扫码 → 可能市集和小红书的契合程度更高；
- 坏消息：使用小红书扫码的绝大多数顾客都无法第一时间找到「扫一扫」在哪里，很多顾客发出了「小红书还有扫一扫？」等疑问；

你有第一时间想到小红书的「扫一扫」在哪里吗？其实国内各大应用的扫一扫位置都不固定。如果说扫一扫大都由业务优先级决定，那么小红书对于线下是否有些漠视呢？

ICYMI：最近在调整每期内容结构，使文本量轻重有度，避免过长。这不是一蹴而就的过程。

最后依然欢迎上周的新订阅者，感谢所有订阅者的支持。

---

# 一些事

**iOS 16.1 电量百分比更新（二）**：继[第65期](https://designscenes.zhubai.love/posts/2170801615631011840)和[上期](https://designscenes.zhubai.love/posts/2183484791448739840#:~:text=%E6%9D%82%E4%BA%8B-,iOS%2016.1%20%E7%94%B5%E9%87%8F%E7%99%BE%E5%88%86%E6%AF%94%E6%9B%B4%E6%96%B0,-%EF%BC%9A%E7%AC%AC65)，这周 iOS 16.1 小更新又改动了电量百分比设计，有点接近之前提到的 A 方案。

![battery - status.png](Scenes%20Weekly%20%2371.assets/battery%20-%20status.png)

 {上图：新 iOS 16.1 Beta 更新后的电量百分比在不同背景上的显示}

作为电量焦虑症患者让电池降到红色很难，但还是试着控制了下电量。可以看到数字字号变大，由 11pt 增加至 12pt（终于不是奇数了）。上次提到 A 方案比较担心对比度是否够大，于是为了考察新电池图标和字体是否使用了 [vibrancy](https://designscenes.zhubai.love/posts/2170801615631011840#:~:text=%E9%A6%96%E5%85%88%E6%8F%90%E5%88%B0%E4%BA%86-,vibrancy,-%E6%B8%B2%E6%9F%93%E3%80%82%E5%AE%83%E9%80%82%E7%94%A8) 渲染，我们来放大查看更复杂背景下的电池图标。

![Battery - check@2x.png](Scenes%20Weekly%20%2371.assets/Battery%20-%20check@2x.png)

 {上图：新 iOS 16.1 Beta 更新后的电量百分比在不同复杂背景上的显示}

可以看到左下和右下电池透明背景后的纹理几乎没有模糊等特殊效果，大概率没用到 vibrancy，很难看清数字，原本的电池显示也同样看不清进度。

不过目前依然是 beta 版本的预览，后续可能会依然更新完善。

---

1、UX Magazine 这篇文章提到一个角度，Snapchat 复杂而又缺少引导的界面，实际上有几点好处：

- 驱逐无趣的成年人，天然形成了一道社区屏障，有着好奇心的青少年总是不缺少折腾劲儿；
- 引起讨论，尤其是 Snapchat 每次添加新功能时，用户会互相讨论玩法；
- 集成游戏化（gamification）的策略，看重长期指标；

实际上第一点很冒险，产品中的难用和易用不再是相对的一面，而是增加了探索感。谨慎学习。

→ [原文](https://uxmag.com/articles/how-snapchat-and-netflix-break-ux-design-principles)还讨论了对 Netflix 自动播放的思考

---

2、英女王葬礼，全英哀悼，市民在伦敦排起了数十万人长队。

说起排队，WIRED 这篇文章从公众科学的角度分析了队列设计。

- 当英国人排队时间超过 5 分 45 秒时，他们会感到烦躁。完美的排队时间不会超过 10 分钟；
- 考验排队有两个指标：
    - 到达速率 (the arrival rate) ：如何尽快到达队尾开始排队；
    - 服务速率 (the service rate) ：如何尽快通过排队；
- 理想情况下，服务速率应大于到达速率；

女王葬礼中，到达速率取决于伦敦地铁和主干路线的客流量承载；服务速率取决于女王的灵车，以及每个人对女王的哀悼仪式。如此队伍越来越长，英国政府网站也只是轻描淡写地警告一下注意会排队。他们可能没有想到的是，正常人持续站立 20 小时后，会开始超出他们的身体极限——[伦敦救护中心（LAS）称](https://www.standard.co.uk/news/uk/queen-london-ambulance-service-st-john-ambulance-london-buckingham-palace-b1025968.html)已为近300名排队群众进行治疗，其中 17 人被送往附近的医院。

同时排队也在考验着路线规划等信息公开与传播效率、安保和无障碍设施的执行。但在那个特殊的日子，十几小时的排队并没有产生太多的动乱。

→ [原文](https://www.wired.com/story/queen-elizabeth-ii-queue/)

💡 拓展：再举一个身边的例子，如下图是北京十号线地铁某双向换乘通道：

![10号线.png](Scenes%20Weekly%20%2371.assets/10%E5%8F%B7%E7%BA%BF.png)

{上图：北京十号线地铁某双向换乘通道，双视角简易图示}

下班高峰期时，右通道经常会挤满人。通道入口即下地铁后换乘的必经之地，出口是一个向上的电梯，很长所以大多数人都会做电梯，即便楼梯那侧没人。红色是向上的台阶。在这个场景里：

- 到达速率由地铁容量、班次间隔决定；
- 服务速率由群众步行速度、上台阶速度和电梯自身速率决定；

到达速率在同一时间段地铁正常运行的状态下基本是固定的。但因为很多人走路看手机，特别是上台阶时走的更慢，又因为大多人都会做电梯，电梯运行速度也不能太快。所以疏通、缓解人流积压是首要的方法。所以地铁工作人员会在 L1 入口处催促提醒人们快点行进。

但实际情况是，L1 阶段即便不分心地行进，通过速率也很快到达上限。原因在于 L2 阶段人们举着手机爬完台阶后走得更慢（可能是向上做功消耗了体力），从而导致后面人想快也快不起来。如果细算的话，L2 其实还涉及到电梯排队中的到达速率，其服务速率则又由地铁班次决定。所以在 L2 这个两个队伍交汇节点处安排地铁工作人员进行有效疏导，比在 L1 效果更明显。可惜这个情形我只见过几次。

---

# 重读HIG（十一）

本节是重读 Human Interface Guidelines 系列连载第十一期，目的为温故知新和跟进新内容。 为避免篇幅过长，不会一次发布太多，之前内容已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上。

## 启动（Launching）

诸如「在用户体验之后而不是一开始就询问应用评分」这类问题不再赘述，因为这节有更加混沌的 launch screen 问题。

如平台需要，则提供 launch screen（启动屏）。事实是除了 watchOS 和 macOS 都需要，LaunchingScreen.storyboard 已经是商店审核的一环。 

在 iOS 的历史中，launch screen 早期是一张位图，原本是用于衔接首屏界面，给用户一种系统快速响应的感觉，所以现在机能的基础下，launch screen 理想情况下是几乎不可见的，因为过渡时间很短（虽然这个时间可控而被用于其他用途）。

![launch_image.jpeg](Scenes%20Weekly%20%2371.assets/launch_image.jpeg)

{上图：早期 iOS 股票应用的 launch screen，左图}

HIG 强调，launch screen 不是onboarding（引导）或 splash screen（闪屏）。[Onboarding](https://developer.apple.com/design/human-interface-guidelines/patterns/onboarding) 后面会讲，但是 HIG 对 splash screen 的定义是什么呢？没找到。

---

先回来看 launch screen，最新的 HIG 依然建议：

> Design a launch screen that’s nearly identical to the first screen of your app.

Launch screen 设计应与接近应用首屏界面。HIG 这里举例了一张我几乎没看到过的 Safari launch screen 界面。

![safari.png](Scenes%20Weekly%20%2371.assets/safari.png)

{上图：Safari launch screen 界面看起来比 skeleton screen 更「进一步」}

- Launch screen 也要匹配系统浅色/深色模式；
- 淡化 launch screen 体验，避免延后进入应用；
- Launch screen 不适合「艺术表达」，“It isn’t an opportunity for artistic expression”；
- 不要打广告；
- 避免在 launch screen 上出现文本，因为该屏无法本地化响应；
- 不要包含 logo 或其他品牌元素，除非这些是应用首屏的固定一部分；
- 不要将 launch screen 设计的像是一个 splash screen 或者「关于」窗口；
    - 此时 HIG 依然没有告诉我们 splash screen 是什么？莫非是将上述建议都反向执行便是 splash screen？

鉴于 App Store 符合这些建议的第三方应用一时难以寻觅，我试着逐帧观察了下 iOS 一些系统应用。

![launch screens.png](Scenes%20Weekly%20%2371.assets/launch%20screens.png)

{上图：iOS 16 Beta (20A5356a) 的七款应用 launch screen 节选}

上面这些是我主观上感知到比较明显的作为 launch screen 用途的界面。首先它们都衔接了首屏界面的背景，可以在左 1 和左 2 中更清晰地感知到。App Store 、健身和计算器都像是无数据状态的首屏界面，不清楚具体如何构成。右 1、右2 和右 3 图中有个细节是，他们都处于「圆角没有完全展开」的状态，说明这三款应用启动调用资源不多，launch screen 时间更短。

---

隔壁 [Material Design](https://material.io/design/communication/launch-screen.html#usage)（后简称 MD）对 launch screen 的定义又不一样。

> Launch screens can be displayed upon an app’s launch from the home screen when an app loads, **instead of displaying a blank screen**. Displaying a launch screen can **decrease the sense of a long load time**, and has the potential to **add delight** to the user experience.

MD 把 launch screen 分为两种：

- 当 launch screen 加载时间过短时，适合使用 Placeholder UI（占位界面）模式，以加快响应感知，更像是首屏的 skeleton screen；
- 其他情况下，可以在  launch screen 上放上 logo 标识提高品牌认知度。同时也要避免出现品牌标语以外的文本；

![MD-LS.png](Scenes%20Weekly%20%2371.assets/MD-LS.png)

{上图：Material Design 2 中的两种  launch screen 分类}

虽然各项建议没有 HIG 详细，但是也给出了详细的定义。然而与 Apple 说明 [Specifying Your App’s Launch Screen](https://developer.apple.com/documentation/xcode/specifying-your-apps-launch-screen) 不同的是，Android 对开发者单独提到了 splash screen 概念，只不过是作为启动界面的 API 出现，而且仅支持 Android 12 及以上版本。[开发文档中](https://developer.android.com/develop/ui/views/launch/splash-screen)这样介绍 splash screen：

- Splash screen 仅在应用进程没有启动过时（冷启动）和 Activity 没有创建（暖启动）时出现，热启动不会出现；
- 和 launch screen 一样在应用准备就绪后消失；

下图是 splash screen 元素和机制说明，124均可单独配置。

![Elements and mechanics of the splash screen.png](Scenes%20Weekly%20%2371.assets/Elements%20and%20mechanics%20of%20the%20splash%20screen.png)

{上图：Android 开发文档中 splash screen 结构说明}

后面更详细的开发先不提，只到这里就看出这和 launch screen 一部分用途重叠……一时间我不清楚想用哪个 meme 表达我的心情。

![memes.png](Scenes%20Weekly%20%2371.assets/memes.png)

{上图：混乱的命名}

---

给这节下一个结论不太容易，最多是冲淡一些经验主义带来的盲区迷雾，对实际工作带来的帮助并不大。但藉此了解 launch screen 背后的目的之后，发现还是殊途同归。无论是加快响应还是品牌表现，都有其合理之处。

→ 本节出自

[Launching - Patterns - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/patterns/launching)

💡 拓展：Graphical User Interface Gallery  - Splashes

[GUIdebook > Splashes](https://guidebookgallery.org/splashes)

---

# 摘录

这周看过的一些——

> In 2011, we launched The Verge. We had a deal with Yahoo, and Yahoo would just send us floods of traffic, and we could never figure out why. I am very opposed to doing too much metrics in the newsroom. I think it distorts — The Verge is about the future, data can only tell you about the past, so if we were to only do what the data says is good, I would only review the iPhone every day for the rest of my life. It would just narrow us completely.

—— Nilay Patel - [An Interview With The Verge Editor-in-Chief Nilay Patel About Building a Destination Site](https://stratechery.com/2022/an-interview-with-the-verge-editor-in-chief-nilay-patel-about-building-a-destination-site/?access_token=eyJhbGciOiJSUzI1NiIsImtpZCI6InN0cmF0ZWNoZXJ5LnBhc3Nwb3J0Lm9ubGluZSIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJzdHJhdGVjaGVyeS5wYXNzcG9ydC5vbmxpbmUiLCJlbnQiOnsidXJpIjpbImh0dHBzOi8vc3RyYXRlY2hlcnkuY29tLzIwMjIvYW4taW50ZXJ2aWV3LXdpdGgtdGhlLXZlcmdlLWVkaXRvci1pbi1jaGllZi1uaWxheS1wYXRlbC1hYm91dC1idWlsZGluZy1hLWRlc3RpbmF0aW9uLXNpdGUvIl19LCJleHAiOjE2NjU4MzQ4NjgsImlhdCI6MTY2MzI0Mjg2OCwiaXNzIjoiaHR0cHM6Ly9zdHJhdGVjaGVyeS5wYXNzcG9ydC5vbmxpbmUvb2F1dGgiLCJzY29wZSI6ImFydGljbGU6cmVhZCBhc3NldDpyZWFkIGNhdGVnb3J5OnJlYWQiLCJzdWIiOiJYbkRxMW9nY1BhQnZWYXk2czR4eGpoIiwidXNlIjoiYWNjZXNzIn0.aO_tyZDlrwvGAtiWOdld9PbZd6CvoPLNjLhwEGSvwKUnCYFOLztxrxU68rpE59JaNBV35sv6MnK1Uc9ArUhHrH88Kr4ild619gv-SKoqwgInRC0urr7xoWM_6BVgGzVYadry32JXotq7nTaw15mGiLN0kvCCGM7D03uazIQBo40PrTU7pX6TrjP50hst57z2twWPG2TNgqcua712B-y5oU8PP_eBt5wrX-b67EH4wLoUzkjW6eHS5AzzTvYDqabfykPFubuMH2bLjaZqLz8AHOSyDNeaumUX2n7ujR3fvdXlxaEDO7keZ7iKORYJ-T9dmWeyUWZYkJDQ2Bx-Yv2JxA)

---

# 还有一些事

1、中世纪的战争和瘟疫，让你可能会有一种彼时人们寿命都很短的感觉，人到而立之年仿佛就要开始迎接死亡。但根据挖掘出的中世纪人骨骼和牙齿所测算的年龄，公元 500 年到 1531 年间的大多成年人都[活到了 50 岁以上](https://onlinelibrary.wiley.com/doi/10.1002/ajpa.22329)，长寿的例子也有不少。造成这种错觉的原因之一是，或许没有分清「平均寿命」和「预期寿命（Life Expectancy）」的数据意义。

- 平均寿命即为统计学意义上的取样平均，计算的是从人出生到死亡的年龄数值；
- 预期寿命代表的是所处年龄段之后的平均寿命，更偏向一种统计期望；

中世纪医疗水平低下，“民科”泛滥，对大多数疾病没有科学地应对方式，特别是婴儿。例如中世纪的英格兰，地主家庭生下的男婴出生时预期寿命只有 [31.3 岁](https://academic.oup.com/ije/article/34/6/1435/707557)，而地主家庭的成年人 25 岁预期寿命有 [25.7 岁](https://doi.org/10.1080/08898480902790387)。这表明，新生儿容易夭折的状况大幅降低了其预期寿命，但是一旦顺利成人，都能活到50岁左右甚至更长（因为是平均值），长寿并不是现代人的特征。

随着医学进步，新生儿陪护和疫苗的发明，让婴儿死亡率大大降低，出生预期寿命也随之提高，例如新加坡新生儿预期寿命就超过了 86 岁。

注：本段与计划生育政策无利益关联。

→ [原文](https://www.sapiens.org/archaeology/life-expectancy-measure-misperception/)

---

2、今年是从 The Verge 出身的记者 Casey Newton 创办 独立新闻通讯 [Platformer](https://www.platformer.news/) 的第二年。两年间他的通讯订阅人数从刚离开 The Verge 时的24,000 人，到第一年的 49,000 多人，再到今年已经 75,000 多人。每年都有几篇热门报道带来了稳定的增速，而大量非热门「中等质量」文章带来的订阅抵消了一些流失用户，类似长尾效应。

![b2ad4946-5bec-4ee8-a357-2f835f78727a_1024x1024 大.jpeg](Scenes%20Weekly%20%2371.assets/b2ad4946-5bec-4ee8-a357-2f835f78727a_1024x1024%20%E5%A4%A7.jpeg)

{上图：Vaporwave portrait of runners on top of clouds, by DALL-E，图源原文，有所裁剪}

文章提到有趣的一点是，时代变了——拜登内阁在 2021 年年初就任，特朗普时代结束。社会话题变少了……Newton 时常陷入选题困难中。当他很久没有写出独家新闻时，他会质问自己：我所做真的值得读者们付费吗？

Newton 没有正面回答这个问题。但问心无愧的是，他和其他独立通讯作者都不会迎合社交网络的偏好去输出内容和观点。并且由于更新频率不低，他不必一次性谈论完自己所有的想法，想法是会变的，在每次变化的过程中，可以让他专注于其他报道可能注意不到的细节角度。

谈到每周四次更新的节奏，连全职写作的他也会感到喘不过气（oppressive）。

另外 Substack 的一些产品更新确实起到了不错的效果，比如[第 55 期](https://designscenes.zhubai.love/posts/2140365736035151872#:~:text=%E8%B7%9D%E7%A6%BB%20Substack-,%E4%BD%9C%E8%80%85%E4%BA%92%E7%9B%B8%E6%8E%A8%E8%8D%90,-%E5%8A%9F%E8%83%BD%E4%B8%8A%E7%BA%BF%E5%B7%B2)提到的作者互推功能，自八月初以来 Platformer 增加了9,000 多名免费订阅者。Substack 的付费预览功能也起到了较好的转化。

→ [原文](https://www.platformer.news/p/how-platformer-is-changing-in-year)

---

3、Colorize Pictures 是一个给单色/黑白老照片上色的网页应用。并可根据照片内容的不同风格选择不同的上色模式。我在 Unsplash 上找到一张样图，转换效果很棒，看到不同颜色大提琴盒了吗？

![PHOTOES.png](Scenes%20Weekly%20%2371.assets/PHOTOES.png)

{上图：Colorize Pictures 对原黑白照片中的衣服、物品、乐器和街头的颜色还原}

→ [试试](https://palette.fm/)

---

4、Mozilla 使用开源工具 RegretsReporter 独立审计用户行为，在分析了 5 亿多篇视频、收集了几千份数据后他们发现 YouTube 的「unwanted」根本没什么用——和大多数人一样。他们选取了 YouTube 上四种不想继续看到某视频方式：

- the thumbs down “dislike” button（点踩按钮）
- not interested（不感兴趣这个视频）
- don’t recommend channel（不要再推荐这个频道）
- remove from watch history（从观看记录中移除）

在这四种方式中，「不推荐频道」是最有效的移除推送相关视频的方式，但也只阻止了 43% 的不推荐视频。「不感兴趣」效果最差，只能阻止 11% 的视频。点踩是 12%，从观看记录中移除是 29%。YouTube 没有公开这个具体算法可能有他的风控因素，但当用户发现 YouTube 的这些设置都没用时，用户反而开始避免点击自己想看的视频。深受其害的我已经有好几年没有访问 YouTube 主页了。

有趣的是 Mozilla 报告中使用的是 [Chubbyemu](https://www.youtube.com/c/ChubbyemuGames/videos) 的视频举例，Bernard 小哥的视频标题风格统一，确实是很好的实验材料（笑）。但其实我还挺爱看的，他们[在 B 站](https://space.bilibili.com/297786973)也有同名官方频道。

→ [报告](https://foundation.mozilla.org/en/youtube/user-controls/)

---

5.1、Failory 这期介绍了 [Peloton 商业模式](https://www.failory.com/blog/peloton-business-model)，他们这[一系列文章](https://www.failory.com/blog#product)写的都挺深入浅出的。

5.2、Canva 推出了 [Canva Docs](https://www.canva.com/newsroom/news/canva-unveils-docs/) 可以集成自家大量富媒体资源，Turner Novak 描绘了 Canva 的[版图](https://twitter.com/TurnerNovak/status/1573025172780716032)。

5.3、iFixit 对 iPhone 14 的可维修性评分[高达 7 分](https://zh.ifixit.com/News/64865/iphone-14-teardown)，玻璃后盖重新的变得便于拆卸。[Teardown Wallpapers](https://zh.ifixit.com/News/65159/iphone-14-teardown-wallpapers) 也出炉了。

5.4、你可能不会加密你的存储设备，但丢失时也要记得彻底擦除信息。如果你的公司如 Morgan Stanley 一样规模，那更要注意硬盘中的信息泄露问题，而不是草率地交给普通搬家公司解决。[大摩为此交了 3500 万美元罚款](https://arstechnica.com/information-technology/2022/09/morgan-stanley-pays-35m-penalty-for-extensive-failure-to-safeguard-customer-data/)——最早可追责到六年前。

5.5、每个国家和地区化身为宝可梦会是什么样？让 Stable Diffusion [告诉你](https://github.com/sradc/each-country-as-a-pokemon-stable-diffusion)。

5.6、知名 YouTube 游戏吐槽家 [videogamedunkey](https://www.youtube.com/user/videogamedunkey) 宣布了自己的游戏发行厂牌 [BIGMODE](https://bigmode.com/)。他们还想建立一个独立开发者的「[互助网络](https://bigmode.com/networking/)」，NICE。Please note: They are not accepting any games that use NFTs, crypto or blockchain.

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

![Railbound.png](Scenes%20Weekly%20%2371.assets/Railbound.png)

{上图：Railbound}

一款修补铁路，环游世界的休闲益智游戏。官方简介如此，我也想不出更多的词句。画面风格如你所见，要做的就是安排铁路路线，让带有不同数字的车厢按顺序与车头接轨。但是不同的铁路机制，让游戏后期远比这画风带给你的预期要难，好在游戏贴心地准备了提示功能💡。

→ [游戏获取](https://store.steampowered.com/app/1967510/__Railbound/)

---

# 映像

现实拟像放映——

![ay6s9ewbysg91.jpeg](Scenes%20Weekly%20%2371.assets/ay6s9ewbysg91.jpeg)

{上图：DALL·E 2生成的拿着十字架自拍的耶稣}

By DALL·E 2.

Prompts: Jesus Christ taking a selfie while on a cross.

→ [出处](https://www.reddit.com/r/dalle2/comments/wkmgz5/jesus_christ_taking_a_selfie_while_on_a_cross/)

---

# 温故

→ [Scenes Weekly #22](https://mp.weixin.qq.com/s/fs8g0sxNJ60qivYrk5rKog)

- 减轻复杂应用中因长时间等待或中断造成的挫败感的五条建议
- 创造力的背后来源于大量练习
- 丑的实验设计
- Google [gallery.io](http://gallery.io) 即将关闭
- 限制言论次数的社交网络平台 Minus 
- 开源 Discord (PWA)，Revolt
- 美国 Android 用户 TikTok 月平均使用时长和 YouTube 的对比
- 杉浦康平作品在线展览
- 远离 Twitter 的「隐居之地」Thoughts
- 非洲传统织物图鉴赏

---

喜欢本文的话，欢迎分享、订阅。

第 70 期请[在此查看](./Scenes Weekly #70.md)。

本次封面使用了 IBM Plex Sans 字体，灵感来自 Nvidia GTC 2022。