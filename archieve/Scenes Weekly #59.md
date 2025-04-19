# Scenes Weekly #59

2022-07-04

\> 设计视角下的世界——

第 58 期请[在此查看](./Scenes Weekly #58.md)。

本期出现：

- 特色鲜明的锦华明朝体
- iPad 圆形光标解析
- Figma 插件更新
- Brave Search 搜索引擎 Goggles 体验
- Robinhood 疯狂一周回顾
- 伯克利人工智能实验室出品的填字游戏 AI
- 其他：第十一届方正奖、即时设计插件 API 开放、GSAP 蜘蛛动画、轻量级的音频剪辑工具 Teapodo、美式杀猪盘短信文学鉴赏、macOS 虚拟机 VirtualBuddy、媒体 Wired 工会罢工

如有格式异常建议点击最上方「在浏览器中访问」。

---

网上冲浪🏄🏻时偶然看到隔壁 Hwang 的[推荐](https://growing.zhubai.love/posts/2141118101784129536)，感谢！

原文里有一句话：

> 不过，我发现提供工具类型链接的 Newsletter 已经非常多了，之后的更新，我会减少相关链接的内容。

这是一个怎样看待「链接」的视角区别，把链接当做每个话题的「谈资」的话，那么链接无关多少，只是作为引子罢了。

例如本通讯有时仅是简单地分享了链接，可能性一是单纯地懒，即便每周有数千字的写作习惯，但依旧没有摆脱七情六欲，亦或者时间紧迫无法继续深入；二是学识阅历不足以支撑拓展到其他信息面。一只正从井底爬向井口的青蛙🐸，把嗑儿唠死了。

另外 Hwang 最近开发了一款分析咖啡和睡眠数据的应用 [Sleep Coffee](https://apps.apple.com/us/app/sleepy-coffee/id1622169968)，「揭开咖啡与睡眠的关系，从而适度调整生活习惯，让爱喝咖啡的你也能睡好觉」。

---

# 杂事

1、因为忙碌拖了好几期 The Type 会刊没看（反正是中奖绝缘体质），最近一口气补了回来。这次想说的是茉莉字型（Mallikātype）的锦华明朝体。

![1670036384683.png](Scenes%20Weekly%20%2359.assets/1670036384683.png)

{上图：锦华明朝体官网介绍的字体特性：温润而不黏腻，古典而不陈旧，平实而特色鲜明}

这款获得纽约 TDC 优秀字体设计奖的宽体字型，设计灵感来源于民国雕版印书《[彊村丛书](https://www.shuge.org/ebook/qiang-cun-cong-shu/)》。扁扁的外形与加密圈所用字母的逆反视觉迥然不同，人文的感觉让我想起了初中班主任的板书。这位物理老师的板书整洁有力，擦黑板的值日生每次都会叫苦。在他的影响下，一部分人也开始学习老师宽体的写法，以示卷面工整。

![1670036386083.png](Scenes%20Weekly%20%2359.assets/1670036386083.png)

{上图：锦华明朝体现有的一些文字节选}

所以就我自己体验来讲，宽体的排版对比普通方块字会压缩一些空间节奏，整体重心更低。例如上图中的竖提（浪、派、哀）、撇（以）、竖钩（子、孔、字）都与正常明朝体有些差异。因为在宽大于高的一个字形中，只有这样才能维持视觉的平衡，并保持宽体的一致性。日和曰字的处理也让人放心，但对于笔画较少的巴和巾字，设计师在扩张中宫时多了一些束缚（← 当然只是个人偏好）。另外在拉宽的时候，类似旬这样的字也让人有些担忧字怀的横纵比例。

The Type 的报道称，锦华明朝体未来会以极粗和极细版作为母版插值生成不同字重，另外还会有常规比例版适应正文排版需求（感觉气质会变……）。目前茉莉字型将会在今年夏季开启众筹，喜欢这款字体的朋友可以到官网留下邮箱跟踪后续消息。

→ 锦华明朝体官网

[Jinhua Mincho · 锦华明朝体](https://mallikatype.com/jinhua/)

---

2、同样来自 The Type 第 45 期的消息，第十一届方正奖设计大赛圆满收官。其中的银奖作品《流水》也让我产生了遐思。[第 31 期](https://designscenes.zhubai.love/posts/2074407394359783424)提到时事通讯平台 [EVERY](https://every.to/) 特色的标题字体替换，如下图。

![1670036387223.png](Scenes%20Weekly%20%2359.assets/1670036387223.png)

{上图：Every 中文章标题一些字体会替换为自己的 Script 字体}

当时我突然想到，那么中文换成草书间字效果会如何呢——不禁期待起来了。看回字体本身，草书为冷门风格，对于现代数码字体而言，小草大概是可读性的上限。正如评委所言，跃然纸上的草书「也能普及大众（对）草书的识别」。

→ 其他获奖字体

[第十一届『方正奖』设计大赛](https://ztds.foundertype.com/index.php/previous_works/index.html)

---

3、Graeme Fulton 这篇文章介绍了 iPad 上的圆形光标。以往我们见到的圆形光标，要不作为移动端触控的视觉反馈，要不就作为在设计预览中模拟触控区域，这些都不是作为光标用途而生，没有系统级的状态映射。

iPadOS 独立后，建立了「触控优先」的一套标准，并且与 Mac 的触摸板手势保持一致。

- 普通光标有着双色结构，可以适应各种屏幕环境。iPadOS 的光标可以根据不同的背景自动切换黑 / 白，来保持高对比度；

![1670036389216.png](Scenes%20Weekly%20%2359.assets/1670036389216.png)

{上图：macOS 中的辅助功能可以自定义鼠标轮廓和填充颜色}

- iPadOS 的光标有着多种形态变化，比如下面的文本光标（I-beam pointer）过渡，比桌面端鼠标丝滑很多；

![1670036391468.gif](Scenes%20Weekly%20%2359.assets/1670036391468.gif)

{上图：HIG 中展示的，光标移过文本区域时变为 I 形}

- 但最具特色的还是光标的磁性效果。HIG 中早已说明设计中的触控区域余地，这里又强调了一次，因为光标经过类似区域会变为区域形状，如下图：

![1670036392663.gif](Scenes%20Weekly%20%2359.assets/1670036392663.gif)

{上图：Figma 应用中演示光标经过交互元素后的效果}

- 磁性光标还可以用在文本区域，当选中一行文本时，会减少因为手滑选中第二行文本的失误。如果移到了已存在的按钮上，则会保留光照效果。更多演示可[详见 HIG](https://developer.apple.com/design/human-interface-guidelines/inputs/pointing-devices#)；
- 当然 iPadOS 中也有无障碍选项来自定义光标，比如：
    - 自定义轮廓颜色、轮廓粗细；
    - 放大光标后，会在光标中间增加原点；
    - 增加对比度；

可以看到，这些光标设计本都是 Awwwards （FWA / CSSDesignAwards）上的常客。但却常常因覆盖系统光标样式对无障碍不友好而被诟病（说实话有些自定义光标样式确实没有必要，又让人难以辨认光标位置）。但设计没有死胡同，感觉 iPadOS 的光标设计也借鉴了网页图标，反过来网页光标在自定义时也可以参照 iPadOS 的审慎。

→ [原文](https://prototypr.io/post/adaptive-cursor-mouse-touch)

[Touch-First Cursor: Round Pointers vs. Mouse Arrows](https://prototypr.io/post/adaptive-cursor-mouse-touch)

---

4、早期 Figma 的插件只能在冗长的列表点选，并且只有插件标题，连个插件图标都没有，使用效率很低，[深有感触](https://dribbble.com/shots/10872753-Try-Some-Figma-Improvements)。后来 Quick Actions 功能缓解了这个顽固症状，如今改版的插件菜单整合了 components、plugins 和 widgets，优先显示最近使用的，折叠所有，并且可以直接搜索安装社区内容。加上了图标，可以在最近使用、已安装和开发中的插件切换。但这个切换使用了 dropdown 形式，不如拿出来当 tab 切换方便。

![1670036393831.png](Scenes%20Weekly%20%2359.assets/1670036393831.png)

{上图：Figma 中插件弹窗}

先前在 FigJam 上的 widgets 现在 Figma 也可以使用，与单人使用的 plugins 不同，widgets 可以多人使用。

→ Figma 六月更新

[What’s new in Figma: June 2022](https://www.figma.com/blog/whats-new-in-figma-june-2022/)

另外，即时设计也在上周正式开放插件 API。能一键导入 Figma 插件挺有「诚意」的（谁来做决策都是如此）。写本文时，插件广场已有 79 款插件。除了官方制作的插件，还有像 Yuan Qing Lim、Yancy 这样熟悉的身影。说句不该说的，官方做个类似 [Automator](https://www.figma.com/community/plugin/1005114571859948695/Automator) 的插件岂不是绝杀（←玩笑）。

> 从今天开始，与即时设计一起打造「中国的插件开放平台」！

这是一件好事，但是动不动上升到国家层面让我有些 emmmm…… 不管有意无意，国家总是意识形态关联，即便狭义也是广阔的共同体，好好在设计领域耕耘不行吗。如无意的话，希望多注意下文案。

→ 即时设计公告原文

[即时设计正式开放「插件 API 」！邀请所有开发者入驻插件开放平台！](https://mp.weixin.qq.com/s/25fPI4XS2oTtK63WCNZ7rg)

后续：即时设计发布公告的两天后，MasterGo 也发布了一篇……「命题作文」，行文像极我学生时期写不出实质内容然后靠典故名言凑字数。大意是我们也有插件广场，但是没提到只有 15 款插件这个事实。

→ MasterGo 公告原文

[https://mp.weixin.qq.com/s/QTCLQEfnZWBYmszpi2gmfQ](https://mp.weixin.qq.com/s/QTCLQEfnZWBYmszpi2gmfQ)

---

# 摘录

这周看过的一些——

> 安德鲁 · 芬伯格在《可选择的现代性》中文版序言中说道，「我们的生活方式已经如此深入地建立在现代技术的基础之上，以至于各种激进的意识形态似乎都难以触及其根本。我们转而需要的是我称之为技术批判理论（critical theory of technology）这样的东西，这是一种深入各种技术系统生活内部的批判」。重新学习亚历山大和他的建筑模式语言，首先便不能抱着如何用它来做建筑的思路，这也是曼弗雷多 · 塔夫里所反对的「操作性批评」（opperative criticism）。书中的许多模式需要与之配套的政治经济体系，并不一定能在当前社会中实现，但这并不是重点。今天我们正身处一个大是大非的时代，自下而上的建造⸺无论是建筑意义上还是社会生活意义上的⸺看似十分遥远而令人悲观，但《模式语言》在操作手法中蕴含的乌托邦指向是切近而朴素的，它提醒我们，是时候让匮乏的想象力重新振作起来了。

—— The Type 第 45 期

---

# 小事

1、搜索引擎 Brave Search 历经一年结束测试阶段正式上线。之前本通讯就数次谈到这款独立搜索引擎，在第 53 期还有 Brave [搜索主管的访谈](https://designscenes.zhubai.love/posts/2135288052800122880#:~:text=Search%20%E7%9A%84%E4%B8%BB%E7%AE%A1-,Josep%20M.%20Pujol,-%E2%80%94%E2%80%94)。

Brave Search 是现在 Brave 浏览器的默认搜索引擎（至少大多数新用户是），独立从头构建索引，注重隐私、用户至上，保持内容的审核透明度（除非法律要求）。产品里最有趣的是 Goggles，可以自定义搜索结果的展现和排序，算法文件托管在 GitHub 上。比如同样搜索关键词我更需要一些科技博客的文章，就可以加上 Tech Blog 这个 Goggles，如下图。

![1670036395086.png](Scenes%20Weekly%20%2359.assets/1670036395086.png)

{上图：在 Tech Blog 中搜索 Zelda，该 Goggles 算法由 Brave 官方提供}

或者在排除 Hacker News 上前 1k 名浏览量的网站中搜索些内容，或者去掉搜索中的 Pinterest 结果，或者不显示那些搬运工网站（小编要失业了）。所有公开 Goggles 不仅可以通过 PR 更新，还可以自己直接在搜索结果中微调。目前看 Goggles 语法基本是正则为主，写过 ClashX 配置文件应该比较熟悉的那种。

→ Goggles 快速入门

[GitHub - brave/goggles-quickstart: Educational material to learn about Goggles and how to create your own.](https://github.com/brave/goggles-quickstart)

→ 更多关于 Brave Search 的介绍

[Brave Search passes 2.5 billion queries in its first year, and debuts Goggles feature that allows users to choose their own search rankings | Brave Browser](https://brave.com/search-anniversary/)

---

2、用 GSAP 做的蜘蛛，虽然有点抽象，但是很好地还原了那种「感觉」。

→ 查看 sandbox

[spider 2 - CodeSandbox](https://codesandbox.io/s/spider-2-t5nqfy?file=/src/index.js)

---

3、Robinhood 的盈利方式是每次用户交易股票、期权或加密货币时，将订单发给做市商，向做市商收取浮动的返点费用，交易波动越大，费用越高，同样注册开户的用户基数越多，Robinhood 的收入也越多。

按照这个角度来看当年 GameStop（GME）事件，Robinhood 应该高兴得不得了。但还有一个问题，Robinhood 用户购买股票后，交易不会立即结算，即使做市商同意卖给他们也得等待 2 个工作日把钱换为股票。买方必须 2 天内交付资金，卖方 2 天内必须交付相应股票，这产生了信贷因素，如果这 2 天里股票有大幅度涨跌都会影响到双方是否退出。

所以实际交易中都会有一个庞大的结算中心来介入处理这种风险，美股是 NSCC（国家证券结算公司）成为中央对手方，也就是做市商会再把订单传给 NSCC 结算。由于 Robinhood 既是 introducing broker 也是 clearing broker（[对外说法详见](https://robinhood.com/us/en/support/articles/whats-clearing-by-robinhood/)），后者身为 NSCC 会员，有义务向 NSCC 提供现金抵押以对抗风险。所以一直以来 Robinhood 自己也希望自家用户买股票时，账面还留有现金。

按照这个角度来看 GME 事件对 Robinhood 产生了巨大的打击，NSCC 向 Robinhood 请求抵押 30 亿美元现金，罗宾汉一时掏不出这么多（已经在 NSCC 那里放了 6.69 亿美元，依然有 30 亿美元赤字。之前根据风险预估准备了 14 亿，但 GME 疯狂让剩下的 22 亿无法填补），又不能被取消清算资格，只能限制用户交易来降低风险抵押。同时也限制了新用户注册——对别的产品来说，短短一晚有 43 万新注册都要乐醒了，对于 Robinhood 来说却只能当一长串数字而已。

以上为美国众议院金融服务委员会对去年年初 GME 事件的调查报告部分内容。委员会建议调整政策以便监管更好地了解散户，加强对 superbrokers 和 资本流动的监管。Robinhood 作为游戏化（Gamification）的典型产品，争议不断，最后自家股票也成了 meme stock，时至今日距离上市当天已跌去七成之多。

→ 你可能不会读的 138 页报告

[Waters and Green Complete Investigation of Meme Stock Market Event; Release Report Revealing the Troubling Business Practices and Inadequate Risk Management Leading up to the Trading Frenzy](https://financialservices.house.gov/news/documentsingle.aspx?DocumentID=409578)

→ 总结内容出处

[Bloomberg - Are you a robot?](https://www.bloomberg.com/opinion/articles/2022-06-27/matt-levine-s-money-stuff-meme-week-was-too-good-to-robinhood)

---

4、Teapodo 是一个轻量级的音频剪辑工具，支持多轨道剪辑和插入 ID3 信息，自带录音。Rust 内核搭配了略具特色的 UI。目前只支持 macOS，未来会支持 Windows、音频片段的淡入淡出和部分导出、内置音频处理等。

![1670036396561.png](Scenes%20Weekly%20%2359.assets/1670036396561.png)

{上图：Teapodo 界面}

→ 官网

[Teapodo: Fast and Easy Audio Editing](https://teapodo.com/)

---

5、以为现在连填字游戏（Crossword）也有 AI 解决方案了，但是查了下之前就已有 [Dr.Fill](https://en.wikipedia.org/wiki/Dr.Fill) 这样的程序。伯克利人工智能实验室（BAIR）的 The Berkeley Crossword Solver （BCS）看起来优于前者。

![1670036397794.png](Scenes%20Weekly%20%2359.assets/1670036397794.png)

{上图：五家出版社的美式填字游戏 BCS 与 Dr.Fill 对比}

BCS 首先使用问答模型生成每道题的答案概率分布，然后使用概率推导，结合本地搜索和语言模型来处理黑白横纵之间的单词答案。虽然具体的技术看不懂，但是可以看到 BAIR 在 2021 年美国填字游戏锦标赛中，拿出 BCS 的问答模型和已参赛多年的 Dr.Fill 搜索系统相结合，夺得了当年锦标赛冠军。

→ [BCS 填字演示](https://berkeleycrosswordsolver.com/)

[Berkeley Crossword Solver](https://berkeleycrosswordsolver.com/)

---

6、美式杀猪盘短信文学鉴赏。最后的总结居然来自《[最新杀猪攻略（2019 年 3 月版）](https://www.reddit.com/r/Scams/comments/njimju/pigbutchering_scam_sha_zhu_pan_photos_of_training/)》😅…… → https://maxread.substack.com/p/whats-the-deal-with-all-those-weird

[What's the deal with all those weird wrong-number texts?](https://maxread.substack.com/p/whats-the-deal-with-all-those-weird)

---

7、上周在 [Newlearner の自留地](https://t.me/NewlearnerChannel) 看到，VirtualBuddy 是一款利用 macOS 自身[虚拟化框架](https://developer.apple.com/documentation/virtualization)的虚拟机应用。也是众多 macOS 同类虚拟机中可视化程度最高的一个，之前无论是 [VirtualApple](https://github.com/saagarjha/VirtualApple) 还是 [MacVM](https://github.com/KhaosT/MacVM) 都需要 XCode 编译。

VirtualBuddy 支持三种 IPSW 安装方法：直接打开、选择官方源下载或自定义网址下载。目前应用还是有些不稳定，我自己下载了 IPSW 后安装失败（内部虚拟化错误），在讨论区也没找到方法，重试几次无果。

→ GitHub 地址

[GitHub - insidegui/VirtualBuddy: Virtualize macOS 12 and later on Apple Silicon](https://github.com/insidegui/VirtualBuddy)

---

8、Condé Nast 旗下媒体 Wired 代表大约 65 名编辑的工会威胁 Condé Nast 管理层，如无法解决薪资问题，编辑们将在 7 月中旬的亚马逊会员日罢工 2 天。媒体通常会在购物节那天推荐各种商品赚取推广佣金，罢工即代表 Wired 编辑即便准备好内容当天也不会发布。

Condé Nast 旗下还有 Vogue、GQ、New Yorker（纽约客）等知名媒体。公会要求至少要与 New Yorker 的作家平起平坐。纽约客于 2018 年成立工会，并已经在 2021 年初进行过一次罢工威胁，最终与管理层达成了协议。媒体编辑维护自身利益而罢工已有多次先例，迈阿密先驱报、彭博社、BuzzFeed、Vox Media 都有过类似罢工事件，有些罢工能够谈拢条件，有些则是直接退出。原因无一例外都是产出和回报不成正比——毕竟谁不想好好过日子而去罢工呢？

→ AXIOS 原新闻

[Exclusive: Wired’s union threatens to strike](https://www.axios.com/2022/06/30/wired-union-strike-threat-conde-nast)

---

> 我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

→ [封面存档](https://figma.fun/f9e6Lk) ([figma.com](http://figma.com))

---

# 劳逸

![1670036399078.png](Scenes%20Weekly%20%2359.assets/1670036399078.png)

{上图：Steam 新品节}

这周的任天堂 mini 直面会带来很多惊喜，不过由于之前鸽掉加上周刊的原因没有及时分享一些 demo 游玩感受，现在补发一下。

[GOODBYE WORLD](https://store.steampowered.com/app/1833490/GOODBYE_WORLD/) ：独立开发者的生存物语； [Last Command](https://store.steampowered.com/app/1487270/Last_Command/)：贪吃蛇与弹幕游戏的有机结合，难度不低。有着高风险高收益的机制，还有着类似 STG 的擦弹技术需求； [14 Minesweeper Variants](https://store.steampowered.com/app/1865060/14/)：规则衍生与变换的扫雷，最后变为数学做题家； [Terra Nil](https://store.steampowered.com/app/1593030/Terra_Nil/)：「年度环保游戏」。众所周知气候一直是国际热议主题，你需要在一片废土上从风力发电机开始，用各种机器逐步还原大自然面貌，这期间需要根据各个建筑的摆放逻辑来拼合地形…… 最后拆除掉这些机器！ [Anger Foot](https://store.steampowered.com/app/1978590/Anger_Foot/)：第一人称迈阿密热线，但是用脚； [Cursed to Golf](https://store.steampowered.com/app/1726120/Cursed_to_Golf/)：谁知道，高尔夫也能和 roguelike 缝合。需要在杆数有限的情况下完成各个小挑战。但我喜欢高尔夫物语的休闲或 What The Golf 的搞怪（高尔夫类游戏确实太多了）。 [SIGNALIS](https://store.steampowered.com/app/1262350/SIGNALIS/)：经典而老派的 PS1 解谜风格，带着抽象 Anime 美少女要素的生存解谜，在这之间还混杂克味。对我来说有多余时间才会考虑正式版。 [Cult of the Lamb](https://store.steampowered.com/app/1313140/Cult_of_the_Lamb/)：艺术风格和动作手感不错，但地图中任务与背景分割不明显。相对比玩法上有些常见，以撒式地牢加上田园传教，cult 到位了。 [九日](https://store.steampowered.com/app/1809540/_/)：同样有着出色的艺术风格和手感，并缝合了后羿神话与 platformer，我对它的期待比 lamb 更高。

→ 新品节的页面依然可以访问

[Steam 新品节 2023 年 2 月版即将隆重登场](https://store.steampowered.com/sale/nextfest)

---

# 映像

现实拟像放映——

![1670036400161.png](Scenes%20Weekly%20%2359.assets/1670036400161.png)

{上图：DALL·E MINI 生成的图片}

随着 DALL·E 2 的发布，一系列图像生成工具走进大众视野。DALL·E MINI 的生成质量不是最好的，但一定是最先发展的…… 有人把它最小化并放到了 PyTorch 里，仅需几行 Python 即可使用同样功能。用 DALL·E MINI 生成各种奇怪图片的 [Weird Dall-E Mini Generations](https://twitter.com/weirddalle) 账号，已经有 100 万的关注者。它太火了以至于 OpenAI 要求他们更改名字，现在是 Craiyon。

→ [ICYMI](https://www.craiyon.com/)

---

# 温故

→ Scenes Weekly #10

[Scenes Weekly | No. 10](https://mp.weixin.qq.com/s/hXnYA2t_lbNEAv3_Yre-5w)

- 科技推文风文本占位生成 Startup Ipsum
- NN/g 新的用户体验成熟度六阶段
- Win 11 初体验迷惑
- 文案对设计的影响
- 高对比的断笔字体 Maro
- 企业里的产品管理层次
- 人们怎样发现新产品的七个渠道
- 韦斯安德森电影的字体美学
- 为植物爱好者准备的网站 HOW MANY PLANTS
- 超过一万名 Freelancer 调查

---

喜欢本文的话，欢迎分享、订阅。

第 58 期请[在此查看](./Scenes Weekly #58.md)。

本次封面使用了しっぽり明朝字体。灵感来自[该视频](https://www.bilibili.com/video/BV1Hf4y1p7tv?t=68.8)中提到的用户体验可追溯到中国古代风水。