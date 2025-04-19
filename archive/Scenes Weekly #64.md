# Scenes Weekly #64

2022-08-08

\> 设计视角下的世界——

第 63 期请[在此查看](./Scenes Weekly #63.md)。

本期出现：

- WAI-ARIA 创作实践中文翻译
- Figma 20 处小更新
- 音频标识记忆模式
- 重读 HIG（五）
- 其他：Apple Store 时间机器、梦工厂开源 MoonRay 渲染器、Google 引号搜索显示优化、
- 现代 ANSI🔥Art 工具、Prompt 交易网站、Pretty Mapp 地图美化

如有格式异常建议点击最上方「在浏览器中访问」。

---

项目不能设计得又快又好又便宜，但是今年夏天可以又闷又热又潮湿。

上周一 Arc 浏览器突然不断崩溃闪退，前一天周日还是正常的。卸载了所有插件、重启应用、注销应用、重启系统和升级系统（到 12.5）均无果。向官方反馈了崩溃报告和控制台日志，对面也不清楚具体哪里出现了 bug（可能无法复现），并推测可能是网络代理问题。回复有点耐人寻味——

> We sometimes encounter server errors in China, and we cannot help with them at this time; our database does not service this region.

然而最终解决方法是，使用 [App Cleaner & Uninstaller](https://nektony.com/zh-hans/mac-app-cleaner) 完全移除（居然有 8 GB 多存储占用）后再安装才解决问题，到目前为止可以正常使用。

现在的 Arc 就像当初的 Figma，两者都在看似成熟的领域挖出了兔子洞。Arc 有一个会员专供的 [Twitter 账号](https://twitter.com/ArcInternet) 用来展示和讨论浏览器的新功能，很多相当酷的功能让人感觉好久没有碰到这种产品了。

然后，欢迎上周的新订阅者们，感谢所有订阅者的支持。

---

# 杂事

1、腾讯适老化 & 无障碍 Oteam 翻译了 WAI-ARIA 创作实践（1.2 版本）的第 3 章 Design Patterns and Widgets。这一章节更贴合实际应用，「介绍了 29 个常见组件的无障碍实现方式，绝大多数组件都附有详细的代码示例，每个示例包含完整的键盘交互实现和指引」。遗憾的是翻译文本只在 W3C 旧式文档界面呈现，W3C 并没有在新版更友好的 [ARIA APG](https://www.w3.org/WAI/ARIA/apg/patterns/) 网站加入本地化。新版网站示例更实时和直观。

→ WAI-ARIA 创作实践 1.2

[WAI-ARIA Authoring Practices 1.2](https://www.w3.org/2022/07/volunteer-translation-apg-zh/Overview.html)

→ 公布原文

[W3C无障碍组件创作实践中文版发布](https://mp.weixin.qq.com/s/7e7oqScdl1CNsha8imv8Fg)

---

2、Figma 去年七月末发布了 30 处高质量的小更新，以改善设计体验，其中大量功能一直沿用至今。今年一月带来 32 个修复和新功能，半年后的夏天他们又带来了 20 处更新，并且全部用视频演示了一遍。对我最实用的应该是按下 shift 后，将选中的图层进行组对齐，而不是内部对齐。

![1670064449870.png](Scenes%20Weekly%20%2364.assets/1670064449870.png)

{上图：鼠标移到对齐图标后，按下 shift 键后会改变图标样式}

如上图，是让四个 emoji 整体在 frame 里居中，而不是四个 emoji 居中。但是无法使用快捷键（shift + option + H 无法触发）。

→ 更多改动

[Little Big Updates: More improvements for design and collaboration](https://www.figma.com/blog/little-big-updates-august-2022/)

---

3、Webflow 这篇博客文章介绍了音频标识（Audio Logo）的重要性，独特的声音可以将品牌与大脑联系起来。法国国家科学研究中心、巴黎高等师范学院和巴黎大学一份[联合论文](https://www.sciencedaily.com/releases/2010/06/100601072644.htm)表明，一般人只需约 10 次即可触发音频记忆，受过训练的人士仅需 2 次，声音的重复是极为有效而快速的记忆学习模式。

人脑中的音频记忆模式以回声记忆机制存在，这些短暂的数秒钟音频记忆被调用的次数越多，记忆的时间越长。此外声音还能激发更深层次的情感反应，这些音频特点都为营销铺好了道路。

比起原文中提到的 Netflix 和闹钟例子，写字楼的电梯广告可以说集齐了这「三神器」，这些每句话仿佛都要唱出来的广告都有几个共通的特点：

- 音乐式语调，并且会选择大众熟悉的音乐；
- 错位或夸张的重音读法，与普通人说话相区分；
- 楼层够高就能一直复读下去；

→ 查看原文更多正事

[Audio logos: what they are, why they work, and how to use them | Webflow Blog](https://webflow.com/blog/audio-logos)

---

# 重读 HIG（五）

本节是重读 Human Interface Guidelines 系列连载第五期，目的为温故知新和跟进新内容。 因为篇幅原因不会一次发布太多，之后会专门整理。

关于[第 60 期](./Scenes Weekly #60.md)提到的下滑刷新手势，今天看 [@sarunw](https://twitter.com/sarunw) 的推文说道，iOS 16 beta 4 中，SwiftUI 的 ScrollView 已支持滑动刷新手势 .refreshable 函数，这可能意味着官方对该手势的承认。

## 布局

- 使用位置表示重要性。将主要的信息放到窗口或屏幕的上半部分，无论是正常观看屏幕或 VoiceOver 都适用；
- 一些很大的集合内容单屏难以放下的话，可以适当展示一些屏外信息，来暗示还有额外的内容。App Store 是好的例子；
- 所有控件最小点击区域依然为 44x44pt；
- iPad 上考虑将控件放置在两侧，方便双手触控；
- 鉴于目前主流 app 依然有在安全区外交互的情况，也发下 iPhone 和 iPad 的安全区域图：

![1670064451651.png](Scenes%20Weekly%20%2364.assets/1670064451651.png)

{上图：iPhone 和 iPad 的屏幕安全区域（蓝色）和边距（粉色）示意}

- iOS 15 引入了 keyboard layout guide（键盘布局），可以帮助开发者更方便地计算弹出键盘后的安全区域布局，如下图为键盘弹出和收回时安全区判断。做设计时如果是指定了常驻底部的元素，那么弹出键盘后如果指定该元素依然浮在键盘上方，开发设置安全区底部绑定键盘区顶部即可。如果是 iPadOS 分屏浏览的话，还有更多问题，详见当初一篇详细介绍的[文章](https://useyourloaf.com/blog/keyboard-layout-guide/)。

![1670064455666.png](Scenes%20Weekly%20%2364.assets/1670064455666.png)

{上图：iOS 15 键盘布局指引}

- macOS 上则注意避免将控件或关键信息放于窗口底部，用户经常移动窗口会导致底部置于桌面之外；
- tvOS 比较特殊，由于电视尺寸的五花八门，HIG 建议留给电视的安全区上下内间距 60px，左右内间距 80px（根据电视宽高特性，不是相同间距数值）。此外 HIG 提供了大量页面模板供填充图片和文本。

![1670064457627.png](Scenes%20Weekly%20%2364.assets/1670064457627.png)

{上图：tvOS 安全区示范}

- 由于自定义程度较小，HIG 连 tvOS 的网格排版也给出了尺寸和间距建议。在各数目列的网格中，内容之间的水平间距（40pt）和最小垂直间距（100pt）是不变的，随着网格宽度指数式减少，网格本身也会变化。有最开始的 16:9 宽幅（2-5 column）变为正方形（6-7 column）最后逐渐缩为类似白银比率的竖向内容（8-9 column）。如下图。

![1670064461403.png](Scenes%20Weekly%20%2364.assets/1670064461403.png)

{上图：tvOS 网格布局中未聚焦内容宽度曲线图，自制}

- 在寸土寸金的 watchOS 界面中，除了四角外都是安全区域，并且内间距仅仅针对内容，像是一些设计卡片还是建议占满屏幕宽度节约空间；

![1670064463764.png](Scenes%20Weekly%20%2364.assets/1670064463764.png)

{上图：40mm 和 44mm 手表的安全区和最小内容间距示意}

- watchOS 中不要在一行中挨着放置超过 2-3 个控件，2 个指的是带文字 label 的按钮，3 个指的是仅包含图形的按钮（比如自定义表盘中的圆形控件）；

→ 本节出自

[Layout - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/layout)

---

# 摘录

这周看过的一些——

> ​在《新自由主义建筑：当代建筑如何成为控制与服从的工具》一书中，建筑理论家道格拉斯 · 斯宾塞（ Douglas Spencer ）对一种极具物质性的介面提出了尖锐批评，即他所称的「新建筑」中的柔和的曲面。这一类型在 Reiser ＋ Umemoto 、 UNStudio 、 Morphosis 、 Mecanoo 、扎哈 · 哈迪事务所、 Foreiggn Office Architects 等建筑师的作品中屡见不鲜。

> 在这样的新建筑中，斯宾塞解读到了经验的模式化，它制造了「新自由主义的凝视」，而这种凝视「不去理解，不去计算，也不去衡量；它接受命令，把自己投射到呈现给它的运动游戏中，在视野中冲浪，陶醉于提供给它的感官自由。」他认为，建筑介面的「顺滑化」使主体的批判能力丧失， 使我们无法将这些空间理解为意识形态的产物⸺历史的和社会的构建之物（故而可以被改变）。

—— Helen Runting（应宁 译）- 碎散的目光，不安分的物件：项目时代的设计作品与设计工作

---

# 小事

1、Michael Steeber 用 Unity 建造了一台 “Time Machine”，不是备份硬盘，而是带你重访四家标志性的 Apple Store。

- Apple Store, Tysons Corner - 2001.05.19 - 可以参观世界上第一家苹果零售店的天才吧；
- Apple Store, Stanford Shopping Center - 2004.10.16 - 最开始以 mini 商店设计开张，然后微软在该购物中心开了家更大型的零售店。2013 年搬迁到更大的空间，微软的零售店则在 2020 年因 4.5 亿美元税前亏损永久关闭；
- Apple Store, Fifth Avenue - 2006.05.19 - 著名的第五大道店，玻璃立方体；
- Apple Infinite Loop - 2015.09.09 - 最开始的苹果总部店，比起销售苹果产品，更多的是销售苹果品牌周边商品，且大多是独家的；

![1670064465413.png](Scenes%20Weekly%20%2364.assets/1670064465413.png)

{上图：Tysons Corner 店货架上售卖的实体软件，包括 Mac OS X 和 Final Cut Pro 2}

→ 穿越

[The Apple Store Time Machine](https://departmentmap.store/timemachine)

---

2、梦工厂动画（DreamWorks Animation）宣布将开源他们的渲染器 MoonRay（Apache 2.0 许可）。该渲染器曾被用于驯龙高手、疯狂原始人和今年未上映的穿靴子的猫 2 等动画，在梦工厂内部已使用超过 10 亿小时。因特尔和微软也参与其中，负责（光线追踪）性能优化和提供云服务（Azure）。

在 [HN 的讨论](https://news.ycombinator.com/item?id=32357470)中有人提到，梦工厂一直是开源的倡导者，多年来为桌面 Linux 开发提供了大量资金，自己开源了 [OpenVDB](https://www.openvdb.org/) 和其他一些小项目。有人看好开源可以让大量使用 MoonRay 的人和独立工作室多起来，利好自家招聘和动画业界工具的发展。但也有人担忧梦工厂失去了动画制作一大优势，但大家都知道，一部动画评价不仅在于制作质量如何，而是媒体艺术的全方位表达。

MoonRay 将在今年晚些推出。

→ 开源官网

[MoonRay Production Renderer](https://openmoonray.org/)

---

3、Google 搜索中加入引号可以显示必定包含此关键词的搜索结果，现在 Google 优化了搜索结果显示，会直接显示该关键词所在上下文，而不是该页面的描述。同时 Google 提示：

- 有时会出现，搜索关键词处于一个无法生成上下文的位置，比如菜单项。此时便不会显示定位文本；
- 关键词在页面没搜到时，可以利用浏览器检查元素工具中的搜索，这样一些弹框里的文本也能搜到；
- 缓存改变；
- 标点符号有时会被视为空格；
- ……

Google 本身的搜索引擎并未改变。

→ 更多

[How we're improving search results when you use quotes](https://blog.google/products/search/how-were-improving-search-results-when-you-use-quotes/)

---

4、Marek Rogalski 的主页时隔 6 年更新了一个小工具，ANSI🔥Art（不是 ASCII ART）。原本 ANSI ART 只能显示 4bit 16 种颜色，以及使用 IBM PC 上的字符集。时代变了，现在的终端可以显示 24bit 颜色和任意 Unicode 字符，ANSI🔥Art 由此而生。

![1670064468041.png](Scenes%20Weekly%20%2364.assets/1670064468041.png)

{上图：测试一张图片转换为现代 ANSI Art 的效果，左边为原图，右边为转换后的图}

Rogalski 的网站自带图片转换器，如上图，放到右边转换后的图，还能看到一些高矮不一的字符，默认为 [JuliaMono](https://juliamono.netlify.app/) 字体。

→ 试试

[https://mrogalski.eu/ansi-art/](https://mrogalski.eu/ansi-art/)

---

5、[第 61 期](./Scenes Weekly #61.md)介绍过 DALL·E 2 一份描述词（prompt）文档，告诉大家如何生成特定风格的图像。更令人惊奇的是，有人做起了 prompt 交易的买卖。Prompt Base 就是这样一个网站，专门售卖针对 AI 的各种描述词，包括 DALL·E 2、GPT-3 和 Midjourney，价格都是几美元。这就是 AI 夜市吗？

→ 围观

[PromptBase | Buy & Sell Quality GPT3 Prompts](https://promptbase.com/)

---

6、Pretty Mapp 是一个开源的美化地图工具，虽然不如 Mapbox Studio 那样功能强大，但是一样可以做出风格化的效果。

![1670064469790.png](Scenes%20Weekly%20%2364.assets/1670064469790.png)

{上图：北京三元桥的风格地图}

→ [网站](https://chrieke-prettymapp-streamlit-prettymappapp-1k0qxh.streamlitapp.com/)

---

> 我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

→ [封面存档](https://figma.fun/f9e6Lk) ([figma.com](http://figma.com))

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) (zhubai.love)

---

# 劳逸

![1670064472460.png](Scenes%20Weekly%20%2364.assets/1670064472460.png)

{上图：PowerWash Simulator 中某物体冲洗前后对比图}

Square Enix 发行的 PowerWash Simulator 有一个奇特的中文名称，冲就完事模拟器。游戏的目的是冲洗干净各种委托，有车、房屋、庭院还有外星科技。看着污垢冲洗干净，心里就会有一种解压、放松的感觉。游戏还能联机游玩。

→ 游戏获取

[Steam 上的 冲就完事模拟器](https://store.steampowered.com/app/1290000/_/)

订阅 PC Xbox Game Pass 也可直接开冲。

---

# 映像

现实拟像放映——

![1670064474112.jpeg](Scenes%20Weekly%20%2364.assets/1670064474112.jpeg)

{上图：2020 年喜剧宠物摄影奖，猫猫组获奖冠军}

「Why are you upside down Mum?」

© Malgorzata (Gosia) Russell

→ [今年提名](https://www.comedypetphoto.com/gallery/finalists/2022_finalists.php)

---

# 温故

→ Scenes Weekly #15

[Scenes Weekly | No. 15](https://mp.weixin.qq.com/s?__biz=Mzg3NzYwNDEzOQ==&mid=2247484129&idx=1&sn=e32a5f233417a43124de41b373632583&chksm=cf213ea5f856b7b30a77c0e83531148e9d21eea3055eed34a689e5d635855d6a2d0c841d99f6&token=807779442&lang=zh_CN#rd)

- 工信部《互联网应用适老化及无障碍水平评测体系》
- iOS15 Safari 改动
- Apple Style Guide 苹果文案写作指南
- Tweet Deck 时隔 20 月更新
- Mobbin.design 改版
- a11y 资源
- Twitter 在灰度测试评论 up/down vote 功能
- Airpods 收入在各大科技公司中的对比
- 麦金塔的古早说明书
- Piedmont Art Walk 新标识
- Clubhouse 对公众开放
- 斗鱼发布了斗鱼追光体

---

喜欢本文的话，欢迎分享、订阅。

第 63 期请[在此查看](./Scenes Weekly #63.md)。

本次封面使用了 Chomsky 字体。