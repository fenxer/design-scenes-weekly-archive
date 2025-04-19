# Scenes Weekly #60

2022-07-11

\> 设计视角下的世界——

第 59 期请[在此查看](./Scenes Weekly #69.md)。

本期出现：

- Arc 浏览器体验
- 重读 HIG（一）
- Google Map 和 Apple Map 五处对比
- Apple Silicon Mac 虚拟机性能测试
- 其他：Raycast Hacking Friday、世界上最高的网页、欧盟的元宇宙观察报告

如有格式异常建议点击最上方「在浏览器中访问」。

---

抱歉，在上期 Wired 工会罢工威胁的新闻中，两处「工会」字样误打成了「公会」。之前和之后一定还有没发现的通假字，请多见谅。

![1670051927379.png](Scenes%20Weekly%20%2360.assets/1670051927379.png)

{上图：摘自《庵野秀明的1214日》下集 48:03}

另外欢迎上周的新订阅者们，感谢所有订阅者的支持。

---

# 杂事

The Browser Company 最近又发送了一波邀请，我也（终于）有幸获得了测试资格。之前在[第 57 期](https://designscenes.zhubai.love/posts/2147988871198887936#:~:text=9%E3%80%81%E6%9C%80%E8%BF%91-,The%20Browser%20Company,-%E5%AF%B9%20Arc%20%E6%B5%8F%E8%A7%88)提到，距离秋季发布越来越近，官方也愈加活跃起来。

![1670051930792.png](Scenes%20Weekly%20%2360.assets/1670051930792.png)

{上图：默认浏览器使用 Arc 后做的 meme}

上次提到的版本号貌似已经重新计数了，我的测试版本是 0.57.0，并基于最新的 Chromium Engine Version 103。像是 [DEX 周刊](https://dex.zhubai.love/posts/2153076095133097984)已经提及过 Arc 使用体验，这次自己使用后，和工作流契合度比较高，名不虚传。

对我来说，Arc 解决了我在 Chrome 使用额外途径获得的功能。比如我在 Chrome 中使用 [nuTab](https://chrome.google.com/webstore/detail/nutab/hbflaeaeaoabekejplknlenmohgoaodj) 来替换 New Tab Page（NTP），以记录一些备忘、常用复制的文本。Arc 自带了笔记功能，将其设置为 Favorite 即可解决类似需求。还有一些临时的图片标注，一般会打开 Figma 或 [tldraw](https://www.tldraw.com/) 处理，Arc 也自带了白板可简略处理。

Chrome 中同时也使用 [Acid Tabs](https://chrome.google.com/webstore/detail/acid-tabs/hgceopemmcmigbmhphbcgkeffommpjfc) 和 [OneTab](https://chrome.google.com/webstore/detail/onetab/chphlpgkkbolifaimnlloiipkdnihall) 来管理标签页，虽然 Chrome 后来自带了垂直标签页展示，但依然不可避免的累加起大量标签，Acid Tabs 的自动分组很理想化，实际体验只会让标签页到处乱蹿。Arc 则可以直接按照不同浏览器场景划分区域，如下图。

![1670051932504.png](Scenes%20Weekly%20%2360.assets/1670051932504.png)

{上图：Arc 的标签页基本结构}

8 个 Favorite 位用于固定最常用的网页，比如 Gmail、Spotify、Twitter 等。它们可以跨 Space 访问。Space 可设为不同场景，例如我分为了四种：日常、写作、工作和（日语）翻译。每种场景的标签页互不干扰。

![1670051933762.png](Scenes%20Weekly%20%2360.assets/1670051933762.png)

{上图：Arc 的 Space 管理，可以自定义主题颜色、名称和图标}

每个 Space 下还可以继续固定该场景下常用的网页，最后才是一些临时的标签页。Space 之间可以使用快捷键切换，整体不复杂，而且好用。

除此之外还有一些感想：

- [第 48 期](./Scenes Weekly #48.md)提到的拾色器也有实装，并增加了对比度和噪点选项。实际选择起来虽然很有趣，但是选择困难这个想挑一个合适渐变背景，需要一些额外的耐心；
- Arc 的返回是全局的返回（可以跨网站返回，但是新网页会消失），[第 45 期](./Scenes Weekly #45.md)也有提到 Apple Music 和 Spotify 的对比，后者就是全局返回，更符合应用整体性的概念。因返回关闭的网页，会被归档为 Auto-Closed 网页，可以随时查看记录再访问；
- 左上角的地址栏可以一键复制网址和对当前网页（或某个位置）截图，截图自动选取的区域可能是依照盒模型选择，很便利。如果想修改 / 查看当前网址，还是快捷键 ⌘ + L 合适；
- 离开正在播放视频的网页，视频会自动变为画中画播放；
- Arc 支持内部多窗口同时查看多个网页，适合大屏幕使用。还有一个 Little Arc 功能，可以打开一个浮动的小窗口；
- 作为一个还在测试中的产品，Arc 也有一些很明显的缺点。比如插件功能非常弱化，虽然大部分可兼容，但弹窗没有适配，半成品感很强；
- Arc 尚没有做浏览器语言本地化，所以目前只能将所有语言翻译成英语；
- 没有摆脱 Chromium 的老毛病，依然会占用大量内存；

上手几天后，常用的快捷键熟悉差不多，基本已用不到 Chrome。继 iOS15 Safari 改版后移动端首先替换 Chrome，Mac 桌面端也跟进了替换。但我觉得 Arc 最聪明的地方是，没有一味的直接否定前人（Google 服务），而是在保障基本权利的同时，一点点过渡和改进。在 [Arc 的新用户引导](https://1drv.ms/u/s!AsiLaLreNo9Kq1q4ySrwBj2PNqY6)流程中，可以近乎无缝地从 Chrome 转移数据。后续的 Arc，是走兼容同步还是全平台独立同步的路线，也让人拭目以待。

→ 官网申请

[The Browser Company | Building Arc](https://thebrowser.company/)

更新：写完这段文字后一天，Arc 更新到了 0.58.0，插件可以右键管理，但依然没有成型的弹窗样式，另外还有插件无法常驻顶部的 bug……

新增了一个 beta 功能 Boost，可以对网站进行定制，包括样式定制、插入和替换内容。最多可以从四个文件入手定制：

- Style.css：页面加载时的样式。不过覆写的等级可能不如脚本，比如一些字体定义样式没试出来；
- Content.js：页面加载时的 js；
- Background.js：后台加载的 js，可以使用 API 的地方;
- Popup.html：Boost 激活时的弹窗内容；

定制后会自动变为本地插件，如下图：

![1670051934981.png](Scenes%20Weekly%20%2360.assets/1670051934981.png)

{上图：插件管理中，New HN 即为刚生成的本地插件}

Boost 大幅度简化了插件制作，并且如此提早上线测试，怕不是要建立自己的「内容壁垒」，这或许是对之后收费模式的一个暗示。目前 Boost 只有编辑器功能，生成的本地文件与 Chromium 插件结构相同，之后大概会做发布与分享流程上的优化？

→ 详见官方说明

[Arc Boosts (beta)](https://browserinc.notion.site/Arc-Boosts-beta-fd9ea0bfb1b54e9c82c2d88182096405)

---

# 重读 HIG（一）

[第 57 期](./Scenes Weekly #57.md)提到 Apple 的 Human Interface Guidelines 有大幅度更新 。最近不是那么忙的时候，就会想着重新读一遍。一方面温故知新，另一方面看看有没有跟进时代的新内容。当然 HIG 内容很多，不能一口气读完也不可能在一期写完，所以干脆就在这里开个「连载」。

顺便发现了一个细节：HIG 中的图片会根据系统 / 浏览器的浅色或深色模式改变图片配色，这是两张图片，独立的配色，并不是简单的混合模式叠加。然而加载效果很生硬，否则也不会那么明显……

![1670051936015.png](Scenes%20Weekly%20%2360.assets/1670051936015.png)

{上图：左边是浅色模式网页，右边是深色模式网页}

## 无障碍

- 无障碍设计要考虑的，不仅仅是障碍人士，而是尽可能处于各种环境下的所有人。比如强光环境下，屏幕即便调到最高亮度，对比度也会不足，正常人也会有视力障碍；
- 不要覆盖平台手势。HIG 指的是一些类似 iOS 右上方滑下访问控制中心的系统手势。虽然 HIG 并没有定义下滑手势为[标准手势](https://developer.apple.com/design/human-interface-guidelines/inputs/touchscreen-gestures/#standard-gestures)，但 Material Design 中却是[官方推荐手势](https://material.io/design/platform-guidance/android-swipe-to-refresh.html#usage)（该死的 Material 3 没有搜索），如今大量主流 App 依然在使用该手势来更新当前页面数据。在数据交互没有摆脱下滑刷新手势的情况下，一些 app 的「二楼」设计就显得极其恶心。另外 iOS 16 中也加入了点按触发 Spotlight（读者指正，主页下滑触发 Spotlight 仍然存在）。至于 "WeChatOS"，那可不敢叨扰；
- 界面会随着辅助功能中字体尺寸的增加而「变形」，除了减少截断文本外，一些拥挤的左右布局可能也要变为上下结构。另外，如果使用的是 SF Symbols，那么图标也会字体一起放大缩小；

![1670051939265.png](Scenes%20Weekly%20%2360.assets/1670051939265.png)

{上图：最近通话列表中的发起 FaceTime 图标随着系统设置缩放}

- 不要仅靠颜色区分对象或者表示重要信息，务必加上文本说明。不同色盲人士对不同颜色的颜色组合区分度不一样。Sim Daltonims 或者各种设计插件都已有类似的视觉模拟，不再赘述；

→ 本节出自

[Accessibility - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/accessibility)

## 应用图标

- 避免在图标上使用文字，除非你的品牌就是文字形式的。文字形式图标不利于本地化，看起来也显得杂乱。特别是「看 XXX」或「玩 XXX」等字样更是无用；
- 注意出血部位，四周圆角。Apple Watch 则是圆形；
- 不要给图标描边，在白色背景上时 iOS 会自动给所有图标加上 1 像素的描边；
- 这章主要的内容是 macOS 的图标设计。Apple 鼓励在设计真实的拟物设计时，使用对应的材料质感。在设计实物图标时，选择应用相关联的熟悉物品来暗示程序功能（XCode 是暗示可以给 App Store 审核人员一锤子吗）。也要注意加入光影增加真实感，保持圆角风格，以及多层网格构造：

![1670051940242.png](Scenes%20Weekly%20%2360.assets/1670051940242.png)

{上图：Big Sur 后的 macOS 图标结构}

- tvOS 的应用图标更特殊一点，为了达成视差效果需要 [Layered images](https://developer.apple.com/design/human-interface-guidelines/foundations/images#layered-images)；
- watchOS 圆形图标要避免使用黑色背景，以防和手表背景重叠。这时就可以让黑色亮一点或者加个描边。Nike NRC 就是个参考；

→ 本节出自

[App Icons - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/app-icons)

---

# 摘录

这周看过的一些——

> Silicon Valley was founded on an ethic of “move fast and break things” and a boundless techno-solutionism. Although this has been somewhat revised [in the techlash post-2016](https://www.tandfonline.com/doi/full/10.1080/23299460.2019.1602817), moving fast is still the imperative, and arguments still abound that technology is value-neutral and that everything and anything profitable should be built. The speed of ethical and regulatory development [continues](https://www.mercatus.org/bridge/commentary/pacing-problem-and-future-technology-regulation) to be outpaced by technological development, incurring massive ‘[ethical debt](https://link.springer.com/article/10.1007/s43681-020-00030-3)’.

—— [Value Beyond Instrumentalization](https://letterstoayoungtechnologist.com/Value-Beyond-Instrumentalization)

---

# 小事

Elon Musk & Twitter 这场戏演到现在既是意料之外又是意料之中，起先的每股 54.20 美元被外界认为低估了 Twitter 价格。几周后科技股下跌，这笔钱又显得「大方」，然而[与资金关联的特斯拉股票](https://designscenes.zhubai.love/posts/2130213690493816832#:~:text=%E4%BA%BF%E5%80%BA%E5%88%B8%E8%9E%8D%E8%B5%84%EF%BC%9B-,125%20%E4%BA%BF,-%E7%BE%8E%E5%85%83%E6%9D%A5%E8%87%AA%E4%B8%AA%E4%BA%BA)也一起跌了。之前造势颇多，而且还与 Twitter 签订了法律合约。退出交易需要一个借口，首先是机器人和 spam 内容，Musk 一方会对 Twitter 问来问去，一旦 Twitter 没有及时提交文件，Musk 便会称 Twitter 没有履行出示义务，以宣称交易无效。然而详细的合约文件表明即使机器人和 spam 超过 5%，Musk 也无法轻易退出交易，他无法证明这个结果对 Twitter 是否产生重大影响（显然不是）。最后 Musk 付出「仅仅」10 亿美元的代价还带动了特斯拉股票一起上涨（以及又会多了几个 meme 数字？），另一边 TWTR 已降为 36.81 美元每股，老员工不断辞职…… 惨字都得用繁体写。

---

1、Raycast 介绍了他们的 Hacking Friday，每周五这一天，每个员工都可以做一些有益于 Raycast 的事。

- 首先早上建立一个 Slack thread；
- 这一天没有会议，不用一直在线；
- 下一周的周一展示结果；
- Hacking 工作量一天不够做完可以拆分，以保持完成一件事的那种成就感或其他正反馈；
- 紧急事项会优先处理，相关人员也可以暂时退出；

→ 原文

[We hack every Friday - Raycast Blog](https://www.raycast.com/blog/we-hack-every-friday/)

---

2、Peter Ramsey 这次没有讲幻灯片，而是对比了 Google Map 和 Apple Map 两款应用基础功能。这场比赛一开始可能就注定是 Google Map 的胜利，因为数据的量级不一样，Apple 会通过不同地图供应商的数据来弥补，然而实际体验呢？Peter 举例了五点。

- 首先当两者都已知一家餐厅已经关闭时，导航至该餐厅 Google 会提示目标门店已关闭，并提供延时的忽略按钮，Apple 地图则会照常显示导航至目的地。Google 地图的提醒更人性化一些；
    - 但我有点认为这是一个非典型的上下文设计案例，餐厅既是享受服务的目的地，又可当做一种地标识别。所以虽然 Google 地图体验更好，但也不是不能理解 Apple 地图的角度——把结果交给用户自己判断。但不管怎么说，理解上下文设计是产品中很讨好的点；
- 当搜索关键词宜家时，Google 展示了方圆 100 英里内的所有宜家，并按照距离排序好。Apple 是直接显示距离最近的宜家，但这是错误的搜索结果。Apple 的地图数据质量较差，却又那么自信；
- Google 地图支持一些步行捷径，Apple 地图的导航路径依然在主干道路上；

![1670051941249.png](Scenes%20Weekly%20%2360.assets/1670051941249.png)

{上图：Apple Map 和 Google Map 导航路线对比}

- 导航语音是 Apple 更胜一筹，Google 的语气波动不大，无感情的机器人；
- Google 地图有时会无法识别停车场，低频场景但发生了又很头疼；

→ 原文

[Apple Maps vs Google Maps (UX analysis) 🗺](https://builtformars.com/case-studies/maps)

---

3、来看看世界上最高的网页——

> 歡迎您訪問世界上最高最長的網頁! 目前這個網頁高 18.94 千米所以滾動這網頁是一種疯狂的娛樂。祝您有很多樂趣。

→ 查看乐趣

[https://worlds-highest-website.com/zh/#pos1](https://worlds-highest-website.com/zh/#pos1)

---

4、[上一期](https://designscenes.zhubai.love/posts/2155579229599776768#:~:text=%E8%87%AA%E7%95%99%E5%9C%B0%C2%A0%E7%9C%8B%E5%88%B0%EF%BC%8C-,VirtualBuddy,-%E6%98%AF%E4%B8%80%E6%AC%BE)提到 VirtualBuddy 利用了 Mac 虚拟化框架构建。我敬爱的 Mac 大师 Howard Oakley 这次分析了 Apple Silicon Mac 该虚拟化方法的性能。

Mac 提供两个级别（level）的虚拟化支持，一是使用 [Hypervisor](https://developer.apple.com/documentation/hypervisor/apple_silicon)（VMM）技术的 Parallels、VMware 等商业虚拟机产品，是需要大量代码工作量来填充的中间软件层；二是新的 [Virtualization](https://developer.apple.com/documentation/virtualization/virtualize_macos_on_a_mac) 技术，拥有更高的级别，已支持多种关键服务，而且相当轻量化。

Howard 的测试环境是 macOS 12.5，并且使用 Xcode 14 Beta 编译。绕过复杂的 [VirtIO 理论](https://eclecticlight.co/2022/07/06/virtualisation-on-apple-silicon-macs-2-how-does-it-work/)，结论为：

- 虚拟机 CPU 的性能与主机（原系统）相似，无法测试 GPU 性能但 Apple 称虚拟机也可用上满血的 Metal 性能；
- 写入速度约是主机的 10%，读取速度略高于主机的 50%；
- 即使没什么权限限制也无法登录 Apple ID 或 iCloud 服务；

总之，Virtualization 提供了出色但有限制的虚拟化性能。Howard 最后也推荐了 [VirtualBuddy](https://github.com/insidegui/VirtualBuddy)。

→ 原文

[Virtualisation on Apple silicon Macs: 1 How well does it work?](https://eclecticlight.co/2022/07/04/virtualisation-on-apple-silicon-macs-1-how-well-does-it-work/)

---

5、欧盟的这份元宇宙观察文件《Metaverse: Opportunities, risks and policy implications》现在看显得姗姗来迟。报告不长，里面提到了元宇宙的特征：

- 真实性：人们可以沉浸在虚拟世界中；
- 通用性：一个虚拟身份适用于多个设备的多个虚拟平台；
- 互通性：不同系统平台间可以无缝交换信息或交互；
- 可扩展性：网络架构足够强大，高访问量不会影响用户体验；

此外报告也体现出对个人虚拟数据保护的担忧，并谈到了一些政策可能性。经济一节中提到了字节跳动的 Pico 和阿里巴巴的 Nreal 投资。

结论为，元宇宙既带来了机遇，也带来了风险。因商业竞争、数据保护、责任落实、去中心金融、无障碍等问题尚不清晰，欧盟依然处于观察中。欧盟委员会副主席特别强调了元宇宙对反垄断监管机构带来的新挑战，议会已经开始考虑元宇宙的影响。

→ 报告

[Metaverse: Opportunities, risks and policy implications | Think Tank | European Parliament](https://www.europarl.europa.eu/thinktank/en/document/EPRS_BRI(2022)733557)

---

> 我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

→ [封面存档](https://figma.fun/f9e6Lk) ([figma.com](http://figma.com))

---

# 劳逸

![1670051942627.png](Scenes%20Weekly%20%2360.assets/1670051942627.png)

{上图：Last Call BBS}

誉满解密游戏圈的 Zachtronics 迎来了最后一部作品，在 Last Call BBS 里留下了八款一如既往精致的解谜游戏。虽然是「8 合 1」，但是每个小游戏都足够玩上一段时间。比如 Dungeons & Diagrams 玩着不顺的话，平均每关都得至少 30-60 分钟，只一个小游戏就得花费数十小时——

- Sawayama Solitaire：一次性过牌的空当接龙（正常是可以无限翻，间隔为 3、2、1）；
- Dungeons & Diagrams：[数织](https://zh.wikipedia.org/zh-cn/%E6%95%B8%E7%B9%94)改编的小游戏，有着额外的规则，上头；
- 20th Century Food Court：类似 [Automachef](https://store.steampowered.com/app/984800/Automachef/) 和[信号法则](https://store.steampowered.com/app/1577620/_The_Signal_State/)，但是 Zach-Like！
- STEED FORCE Hobby Studio：来拼胶！
- Kabufuda Solitaire：[Eliza](https://store.steampowered.com/app/716500/Eliza/#app_reviews_hash) 中的纸牌游戏，同样很靠运气；
- X’BPGH: The Forbidden Path：设定每步 seed（干细胞？）的行为和方向，最终进化到相应有机物，风格很 cult；
- HACK*MATCH：[EXAPUNKS](https://store.steampowered.com/app/716490/EXAPUNKS/) 里面的小游戏，只不过也像素化了，并且可以联机；
- ChipWizard™ Professional：[深圳 IO](https://store.steampowered.com/app/504210/SHENZHEN_IO/) Alter 版本，还没细研究；

团队解散，不代表创始人 Zach Barth 不再做游戏。在 Kotaku 的采访中提到，Barth 原来是高中微机老师，热爱教学。希望能在其他 side project 里看到 Zach 的影子。

游戏也登录 PC Xbox Game Pass，Steam 也当支持。

→ 游戏获取

[Steam 上的 Last Call BBS](https://store.steampowered.com/app/1511780/Last_Call_BBS/)

---

# 映像

现实拟像放映——

![1670051944224.jpeg](Scenes%20Weekly%20%2360.assets/1670051944224.jpeg)

{上图：废旧商品组成的装置}

Credit Card Destroying Machine

©Michael Landy

---

# 温故

→ Scenes Weekly #11

[Scenes Weekly | No. 11](https://mp.weixin.qq.com/s/qx50IC-BKnF-6Sp26Wg_jQ)

- 2021 Material Design Awards 提名
- cemre 抨击了 Google Map 是如何在 OKR 的驱动下，变得繁琐冗杂，不及 Apple Map（巧了是不是，看待问题的角度不同，结论也会相悖）
- 微信简中官网更新
- 日文字体术语图示
- YouTube Shorts 吐槽
- 我经常看的 Creativerly 写了自己的回顾
- Figma 去年六月下旬的 30 多个更新
- 纽约卡内基大厅的标识重设计
- Dahlia 中意大利新艺术运动的浪漫和优雅提现
- Safari 15 改版批评
- Rive 增加了云端渲染功能，最近他们加入了 Mesh 网格控制，收费也有所变化

---

喜欢本文的话，欢迎分享、订阅。

第 59 期请[在此查看](./Scenes Weekly #59.md)。

本次封面使用了 Inter 和 SF Mono 字体。