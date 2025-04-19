# Scenes Weekly #56

2022-05-30

\> 设计视角下的世界——

第 55 期请[在此查看](./Scenes Weekly #55.md)。

本期出现：

- COLRv1 彩色字体标准介绍
- 低技术界面回顾
- Instagram Sans 特色鉴赏
- Font Matrix 字体匹配参考思路
- 其他：Microsoft Store App Awards、生产力效率迷思、Monterey 隐藏的显示器校准

如有格式异常建议点击最上方「在浏览器中访问」。

---

下周端午假期，可能会不更新，看北京疫情状况。

- Boardcom 将以溢价 49% 的 610 亿美元现金收购 VMware，仅次于微软收购动视暴雪。收购后 VMware 永久许可模式将改为订阅模式。
    - HN 上的 VMware 员工和其他人都对 Boardcom 的利益追求而减少研发投入感到担忧。
- 另一边爱奇艺开源节流 + 涨价效果明显，Q1 净利 1.691 亿元，会员营收增加。
- 你的每一分钱都在推动虚拟化和长视频行业发展，大家都有美好的未来。

---

# 杂事

1、[第 40 期](./Scenes Weekly #40.md)提到 COLRv1 字体的支持，CSS-TRICKS 这篇文章更为详细介绍了网页中彩色字体的发展。

彩色字体最早出现在 19 世纪 40 年代，第一款数字彩色字体可以追溯到 1982 年未公开发售的街机游戏 [Insector](https://www.instagram.com/p/BzIrSryBm_u/)，如今各大浏览器都支持 [COLRv0](https://caniuse.com/colr)，但彩色字体依然并不多见。

如今有四种彩色字体标准，OpenType-SVG、COLR、SBIX 和 CBDT/CBLC。

- SBIX 和 CBDT/CBLC 的 B 即为 Bitmap 的缩写，前者标准由 Apple 主导并用在 iOS 和 macOS，后者是 Google 主导并用在 Android。两者处理的都是位图数据。大分辨率下会变模糊；
- 如果是设计软件本地使用还好，但是过多位图数据导致字体体积膨胀，显然不适用于网页；
- OpenType-SVG 支持渐变样式、图层化、蒙版甚至位图。在这些功能的背后，却不适用于一些基本的字体技术，比如 hinting 和可变轴；
- COLRv1 弥补了 v0 的一些缺陷，使之更接近 OpenType-SVG 的样式标准，同时支持可变轴；
- Chrome 98 和 Opera 86 以上的版本均已支持 COLRv1，Firefox 尚未支持但预计也快了，Safari 可能就看 Apple 心情了（？）
- Figma 对 COLRv0 支持还不完整，Sketch 支持；

早年的 font-palette 依然适用于 COLRv1，既可以用 base-palette 去选择字体设计师的默认色板，也可以使用 override-colors 去自定义每个图层的颜色。

- 限制 1：override-colors 不支持 CSS 自定义属性；
- 限制 2：palette 之间不能插值过渡，颜色是瞬间变换的；
- 限制 3：[浏览器支持](https://caniuse.com/css-font-palette)依然有限；

→ 详见原文

[COLRv1 and CSS font-palette | CSS-Tricks](https://css-tricks.com/colrv1-and-css-font-palette-web-typography/)

→ Webkit 博客也有一篇介绍

[Customizing Color Fonts on the Web](https://webkit.org/blog/12662/customizing-color-fonts-on-the-web/)

---

2、低技术（low tech）代表了更经典，更贴近自然的一个回归方向。那时的设备界面通过 LED 灯或者简单的显示器传达信息，通常不会太复杂，且各部分主次对比明显。像是之前很多设计师所称赞的 TX-6 混音器：

![1669800085314.png](Scenes%20Weekly%20%2356.assets/1669800085314.png)

{上图：TX-6 的屏幕状态设计部分截取}

今天用户界面的很多元素也是从物理交互设备发展而来，在以触屏为主的时代，Jonathan Kendler 总结了低技术界面的一些优缺点：

- 触觉反馈是一项优势，不依靠视觉，形状大小纹理等都可以来帮助用户区分开不同的控件。这点在车机界面领域中讨论已久；
- 逻辑不会太复杂，成本更低廉，易于开发，不必使用类似 Qt 那种昂贵的开发框架；
- 现代的触屏更易出现损坏，坏点遮挡字符、电池寿命短等；
- 相比现代触屏设计的「无限画布」，传统设备有着更多的限制约束，反过来可以让设计更加专注于核心部分；
- 缺点是在本地化方面比较困难，迭代的灵活性差。有时还会让用户误认为产品真的是过时的技术（在家电领域比较常见）；

其实我更想看，低技术的工业设计元素是如何过渡到现代界面设计的这种系统性文章。十几年前，Bret Victor 也有过[类似畅想](http://worrydream.com/ABriefRantOnTheFutureOfInteractionDesign/)，认为未来的交互不是局限于一根手指——实际上我们有十根手指，有很多关节和肌肉，有各种抓握方式——目前的划玻璃只是一种过渡。然而原文依然没有给出未来交互的一个蓝图，亦或是发散的解决方案。这确实有些难以思考。

→ 原文

[The forgotten benefits of “low tech” user interfaces](https://uxdesign.cc/the-forgotten-benefits-of-low-tech-user-interfaces-57fdbb6ac83)

---

3、Instagram 最近进行了品牌升级，这次升级背后有 3 个指导目标——

- 独特的新字体；
- 保持渐变的活力，更加多样化；
- 跨渠道的品牌系统；

![1669800088912.png](Scenes%20Weekly%20%2356.assets/1669800088912.png)

{上图：Instagram 品牌字体展示}

Instagram Sans 是这次升级的重要一部分。由 Colophon Foundry 协助制作，最大的特色在于 一些替换字形来源于 ins 长久以来的手写体 logo，官方称之为 "Flipped the script"。里面还融入了 logo 图形中的圆角矩形基因，这在一些等宽字体中比较常见，并散发着 Grotesque 味道，甚至做了三种不同的 @。

![1669800091558.png](Scenes%20Weekly%20%2356.assets/1669800091558.png)

{上图：Instagram Sans Regular 中 iJOQC 四个字母、@ 的替换和三个独立 logo 图标}

Instagram Sans Script 的加入让整套字体的杂糅性更上一层。其中大写字母 I 也是可以替换的，但估计只有放在 instagram 单词中才能看出来是 I 吧……

![1669800093197.png](Scenes%20Weekly%20%2356.assets/1669800093197.png)

{上图：←左：大写字母 J；↗右上：夹杂替换的 Instagram Sans 拼写；↘右下：Script 基础字型}

具体用法可能像本节第一张图一样，在一些字体 sticker 中随机替换为 Script 字型。针对竖视频还有 condensed 版本，满足了大部分场景使用。

→ 字体介绍

[Instagram Sans Typeface | Instagram’s Brand Refresh | About Instagram](https://about.instagram.com/brand/type)

→ 品牌改版介绍

[Behind Instagram’s brand evolution: Movement, inclusivity and a new purpose](https://design.facebook.com/stories/behind-instagrams-brand-evolution-movement-inclusivity-and-a-new-purpose/)

---

4、Oliver Schöndorfer 有自己的字体配对思路，他称之为 Font Matrix，主要是寻找衬线和无衬线字体间的一些匹配和谐点。这一系统基于 [Indra Kupferschmid 的研究](https://kupferschrift.de/cms/2012/03/on-classifications/)，分三步走：骨、肉、皮。

一款字体的「骨」可以理解成它的字形（可能反过来更好理解）。Oliver 将此分为了三部分：动态的（dynamic）、理性的（rational）、几何的（geometric）。

![1669800094741.png](Scenes%20Weekly%20%2356.assets/1669800094741.png)

{上图：用 a 解释三部分含义}

如上图，动态的即代表倾斜的轴线和较为开放的开口（aperture），理性的即代表垂直的轴线和较为封闭的开口，几何的则代表更加线性、规则的笔画。以 Megatypos 为例：

![1669800096324.png](Scenes%20Weekly%20%2356.assets/1669800096324.png)

{上图：三种「骨架」的字体}

然后是「肉」这一步，开始区分衬线和笔画对比的有无。是否有衬线好说。除此，笔画粗细有致便可称之有对比度的（contrasting），笔画的粗细几乎没有变化，便可称之线性的（linear）。

区分好备选字体的这些特性之后，就可以整理归纳 Font Matrix 了。

![1669800098185.png](Scenes%20Weekly%20%2356.assets/1669800098185.png)

{上图：动态、理性、几何和对比性衬线、线性衬线、对比性无衬线、线性无衬线组成的 3*4 矩阵}

如上图，就像多相配色一样，竖向选择字体搭配，因为有相同的骨架而和谐。想要对比冲击强一点的可以选择骨肉互不相同的字体。但唯独横向选择「肉质」相同的字体会导致难以区分，无法脱颖而出，还会让人感到一种形似同一字体而又不是的紊乱感。

Font Matrix 只是一个参考的出发点，除此之外还要考虑：

- 是否符合你的项目调性；
- 如何安排排版；
- 两者的字面比例、x-height 高度、字重等是否也匹配；

最后的「皮」不参与上述 Font Matrix，但要求你更精细化地描述字体，以对应到需求场景中。

Font Matrix 虽然不适用于所有字体混合排版场景，但是却提供了一个更加亲民化的思路，这里无需繁杂的字体术语，只需几个简单的识别技巧便可做出参考。

→ 原文

[Font Matrix – See & Pair Typefaces Like Never Before - Pimp my Type](https://pimpmytype.com/font-matrix/)

---

# 摘录

这周看过的一些——

> Ironically, the best way to secure top talent is to give them optionality. Whether it's being remote-first, encouragement of side projects, or not locking them into crazy vesting cycles... Be a magnet, not a jail.

—— Steph Smith - 出处

[登录 Twitter，关注Steph Smith](https://twitter.com/stephsmithio/status/1492960024741572608)

---

# 小事

1、Build 2022 上除了云服务的念叨，Microsoft Store 也占了一些戏份，自 Windows 11 发布以来一直备受重视。未来增加的新功能包括：

- Windows Search 中的搜索结果入口；
- 多设备恢复安装；
- 通过 Pop-up store 更便利地推广商店产品（是否指的是 pop-up 形式的商店？）；
- Microsoft Store Ads 搜索和相关推荐广告来了；
- Win32 和 PWA 应用的上架和流程优化；

另外他们也推出了 Microsoft Store App Awards，分为社区提名和编辑推荐两种，并按照不同类别的 App 单独评奖。作为第一届微软官方认证的产品奖项，除了对微软设计语言的偏好外，一些奖项似乎在回应那些，多年来「默默无闻」为普通用户撑起巨大便利的应用。

- 像是老牌截图工具 ShareX、网速测试工具 Speedtest、开源文件管理器 Files、新时代 U 盘启动工具 Refus 等，都拿到了奖。

Editor’s Choice 则是一些服务并满足了大量用户以及一些小众需求的应用。比如 [Talk for Me](https://apps.microsoft.com/store/detail/talk-for-me/9WZDNCRDM04G) 这种科技向善的免费应用，可以替发声障碍人士拼出声音。其他获奖的还有 Disney+、Spotify、Canva、Wondershare Filmora、LiquidText、Discord。

→ 详见原文

[Announcing the Microsoft Store App Awards Winners!](https://blogs.windows.com/windowsdeveloper/2022/05/27/announcing-the-microsoft-store-app-awards-winners/)

---

2、鉴定一下网络热门生产力疑问——

- 凌晨 4 点起床更有效率吗？
    - WSJ 确实报道过相关新闻，工作效率高可能是因为别人还在睡，也不会分散注意力，自然效率高;
    - 重点是 4 点起床是否剥夺了睡眠时间；
    - 有天生的早起者；
- 我们不都是一天 24 小时吗？
    - 模仿成功人士的作息并不一定适用于每个人，每个人都有自己的高效率时间段；
    - 一些非生产力场景，比如成功人士可以雇人家政，但是一般人就要额外腾出时间自己打理；
- 越忙碌代表效率越高吗？
    - 多个任务之间切换处理会降低单个任务的效率，注意力和工作记忆是有限的；
    - 生产力是和质量而不是数量挂钩的；
- 工作时就要保持高兴的心情吗？
    - 幸福感确实可以提升生产力，但两者并不对等；
    - 经常快乐工作的员工受挫时更容易崩溃和感到疲惫，甚至会更自私；
    - 恐惧、愤怒、压力和嫉妒等负面情绪也可以让人在某种情况下提高效率；
    - 像「微笑服务」那样强迫员工保持高兴心情的，适得其反；
- 努力就会有回报吗？
    - 成功的因素里不是最大但最关键的，是运气，不是工作量；
    - 陈年鸡汤，不多说；

→ 详见原文更多外部引用资料

[A neuroscientist debunks the biggest productivity myths | BBC Science Focus Magazine](https://www.sciencefocus.com/the-human-body/productivity-myths/)

---

3、在 macOS Monterey 中，原本显示器偏好设置中的校准不再存在，取而代之的是不直观的自定预置和微调预设，如下图。

![1669800099966.png](Scenes%20Weekly%20%2356.assets/1669800099966.png)

{上图：macOS Monterey 中显示器预置下拉菜单}

实际上，原本的显示器校准程序并未彻底删除，app 隐藏在该路径中：

/System/Library/ColorSync/Calibrators

按住 ⌥ option 键双击打开该 app 便可进入「专家模式」，与普通双击打开不同，专家模式增加了灰度系数（Gamma）的相关设置。

![1669800102130.png](Scenes%20Weekly%20%2356.assets/1669800102130.png)

{上图：熟悉的显示器校准助理界面又出现了}

新建好的颜色配置文件在色彩同步实用工具【设备 - 显示器】里能看到。

→ 详见原文更多校准说明

[Calibrating your display in Monterey](https://eclecticlight.co/2022/05/23/calibrating-your-display-in-monterey/)

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周更新了 0 个。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

---

# 劳逸

![1669800104672.png](Scenes%20Weekly%20%2356.assets/1669800104672.png)

{上图：命途 banner}

いのちのつかいかた（命途 / The Use of Life）主体是简单的 CRPG，但比起废都物语少了很多设定。战斗是回合制的 QTE 博弈。每回合各出三招，在敌人重攻击时躲避伤害，在空档期输出。考验反应和节奏，容错率较低，因此成就感也比较足。目前还是 EA 状态，内容大概 4h 以内。

→ 游戏获取

[Steam 上的 命途](https://store.steampowered.com/app/1483370/)

---

# 映像

现实拟像放映——

![1669800108291.jpeg](Scenes%20Weekly%20%2356.assets/1669800108291.jpeg)

{上图：chess-piece，一枚略有破损的象牙棋子，戴着花冠的女王左手拿着喇叭，右手捂脸}

© The Trustees of the British Museum

---

# 温故

→ Scenes Weekly #7

[Scenes Weekly | No. 7 (SP)](https://mp.weixin.qq.com/s/rYpznKNQqbTgbMfMJnGQxQ)

- 网页设计工具 Graphite
- Collletttivo 发布了 Apfel Grotezk 字体
- 随性的建站工具 mmm
- Mockups 工具 Previewed
- MAP OF THE INTERNET 2021
- iOS Chrome 浏览器桌面小组件思路

---

喜欢本文的话，欢迎分享、订阅。

第 55 期请[在此查看](./Scenes Weekly #55.md)。

本次封面使用了 Sligoil 字体，替换了小写 s 和 l 样式。这是一款带有 ink trap 的等宽字体。