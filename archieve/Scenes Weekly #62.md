# Scenes Weekly #62

2022-07-25

\> 设计视角下的世界——

第 61 期请[在此查看](./Scenes Weekly #61.md)。

本期出现：

- Universal Sans 2.0 定制版
- 3D 制作网页工具 Womp 浅尝
- Figma 深色模式的背后
- 重读 HIG（三）- 图标
- 数字键盘简史
- 46000 美元重设计了三张网页
- 其他：Notion app 更新、Helvetica The NFT、PowerGlitch 小工具

如有格式异常建议点击最上方「在浏览器中访问」。

---

在微信公众号后台编辑器上排版 newsletter 是每周最痛苦的事情，链接和图片说明文本的样式需要使用落后的「格式刷」一步一步复制粘贴过来，效率低下。第三方的排版工具又过于花哨，难道公众号编辑器兼容那么多格式就是为了那些花花草草的东西吗？

之前[畅想过](https://fenx.work/Redesigning-Inline-Editor-822bccdc66a94182851ac7f7895e86b7)融合 Notion 体验浮动编辑体验的公众号编辑器，但梦醒来后，依然是丑恶的现实。倘若哪天有大量时间和精力（← 很难）把公众号文章归档到某个地方，那么就可能停止公众号的更新，直至哪天编辑器有较大的体验改进。

本区域原本作为「鸽讯声明」，由于上个月连鸽外加一些勘误信息，写着写着逐渐变聊天区，但感觉还不错。最后依然欢迎上周的新订阅者们，感谢所有订阅者的支持。

---

# 杂事

Bionic Reading 更新：[第 55 期](https://designscenes.zhubai.love/posts/2140365736035151872#:~:text=%E4%B8%8A%E7%9C%8B%E5%88%B0%E4%BA%86-,Bionic%20Reading,-%E7%9A%84%E6%96%B0%E9%97%BB%EF%BC%88or)提到对 Bionic Reading 提高阅读效率的存疑，之后其身影出现愈见频繁。但质疑声音一直较少让我很意外，除了 Typography.Guru 的这个[视频](https://www.youtube.com/watch?v=V53tbzy9n9w)。

但终于在上周， Readwise 募集了 2000 多名参与者帮助官方补充了实验数据（是的，Bionic Reading 官方没有拿出任何实验论据），[原文在这里](https://blog.readwise.io/bionic-reading-results/)，隔壁 [Shyrism.News #18](https://shyrz.zhubai.love/posts/2162133924519587840) 也有翻译。结果显而易见——

> 使用仿生阅读阅读速度更快的人数（52%）略高于没有使用仿生阅读的人（48%）。也就是说，那些使用仿生阅读速度更快的人平均每分钟只能读 35 个单词。相比之下，那些没有仿生阅读的人阅读速度更快，每分钟能读到 43 个单词。仿生阅读似乎并没有真正起作用。

---

1、[第 58 期](https://designscenes.zhubai.love/posts/2153040612868980736#:~:text=Dinamo%20Font%20Customizer)提到字体厂商 DINAMO 的定制工具，可以给予购买字体的顾客很多修改权利。最近看到 Universal Sans 2.0 也提供了大量定制选项，除了基础轴体变更外，还可以选择大量变体。

![1670057983666.png](Scenes%20Weekly%20%2362.assets/1670057983666.png)

{上图：Universal Sans 2.0 定制变体一览，BuildID v2.0.40.50.80.30.0.4211122123112121111.01.01.500}

单一字重 100 美元起价。

→ 网站

[Universal Sans](https://universalsans.com/)

---

2、浅尝了下正处于 Alpha 测试的 3D 制作网页工具 Womp，由于是实时渲染，Chromium 103 即便开了硬件加速依然有很大的操作延迟，像是操作云主机一样。

![1670057984672.png](Scenes%20Weekly%20%2362.assets/1670057984672.png)

{上图：Womp 当前界面}

Womp 进一步简化了模型，特别是光照，并提供多种 HDRI 背景。地面和天空也不重要，统一为 Backdrop 管理。对比 Spline 更加 “Figma-like”，也少了挤压、克隆等常用工具，但是渲染后的快速出图效果不错。目前最大的问题还是性能上如何做到即时响应。

→ 网站

[Womp is the new way to 3D](https://www.womp3d.com/)

---

3、Figma 今年 Config 2022 发布了深色模式，对于一个迭代了 6、7 年的设计工具来说并不容易。Figma 最近更新的博客也表示：「深色模式设计最难的事情（之一）是人们认为它很简单」。

Figma 的团队想建立新的工作流一方面更改现在的界面，一方面为之后的新功能拓展打基础，使新入职的成员能够开箱即用地设计和开发新功能。鉴于 Figma 有 10 个产品团队，复杂度比想象的还要高。

下面是 Figma 的语义 token：

```plaintext
## Type | UI Element | Color role | Prominence | Interaction

Type { bg, text, icon, border }

UI Element { default, menu, toolbar, tooltip }

Color role {default, brand, selected, design, figjam, component, assistive, danger, warning, success, disabled, info }

Prominence { default, secondary, tertiary, strong }

Interaction { default, hover, pressed }

```

Figma 之前使用 PostCSS 处理 CSS 变量，其中颜色变量为 5100 余个。由于原本变量和语义 token 并非一一对应，所以全部替换工作需要手动完成。Figma 动员了每个产品团队共 40 名开发工程师，一周内便取得了 80% 进展。团队内部将这一周纪念意义地定为 Dark Mode Week。

最终除了新浅色和深色模式外，还增加了一个调试模式（Debug mode）作为彩蛋。调试模式配备一个奇怪的随机色板，用于检查哪里还没用上语义标记。

![1670057985650.png](Scenes%20Weekly%20%2362.assets/1670057985650.png)

{上图：Figma 调试模式的辣眼睛配色}

剩下 20% 的工作就是不断地测试和打磨。即便上线后，随着新功能添加，也需要不停更新。作为构造深色模式的第一课，最简单的需求中往往有着复杂的答案。这点在之前粘贴机制更新时也体现得淋漓尽致。

→ [原文](https://www.figma.com/blog/illuminating-dark-mode/)

---

4、Notion 更新了移动应用，将 web 视图替换为了原生组件。我又把移动端应用下载回来，确实感觉都不一样了（真的是感觉），甚至有了返回。流畅度真的是应用设计第一要素，即便依然不如 Craft 般优雅。

其他写在更新 log 里的还有：

- database 的分栏视图（依然灰度测试中）；
- 快捷创建列（columns）；
- Jira、GitHub、Figma 内联链接预览优化；

→ [日志](https://www.notion.so/releases/2022-07-20)

---

# 重读 HIG（三）

本节是重读 Human Interface Guidelines 系列连载第三期，目的为温故知新和跟进新内容。 因为篇幅原因不会一次发布太多，之后会专门整理。

## 图标

- 一个界面图标要简洁、可识别，暗喻的功能能被认知最好，不应过于复杂（然而大家都知道的事情，有时就是很难贯彻执行）；
- HIG 中的图标调整示例，除了视觉面积的角度外，还有点像字体排版时考虑重心和视觉尺寸：

![1670057986590.png](Scenes%20Weekly%20%2362.assets/1670057986590.png)

{上图：一些异形图标排版对比}

![1670057987503.png](Scenes%20Weekly%20%2362.assets/1670057987503.png)

{上图：根据图标重心单独调整内间距}

- 图标也需要根据当地习俗、文化而本地化。如下图举的两个例子，左边是拉丁字母 A 作为图标时的更换，日语是【あ】，希伯来语是【א】。右边是文档图标中根据阅读顺序 LTR 和 RTL 的不同而有着不同的线条排布；
    - 发散一下，本地化这一点其实在各个编辑器图标中没有体现，比如代表加粗、倾斜、删除和下划线的四个字母 BISU 都没有变为「粗、斜、删、下划」；

![1670057988639.png](Scenes%20Weekly%20%2362.assets/1670057988639.png)

{上图：SF Symbols 中的 A 和文档图标本地化替换}

- 设计图标时避免使用 Apple 硬件产品外观，因为硬件产品外观更新后，图标会显得界面过时。不过看来 emoji 的设计 🎧 （Unicode: U+1F3A7） 不考虑在内；

![1670057989584.png](Scenes%20Weekly%20%2362.assets/1670057989584.png)

{上图：Apple Color Emoji 中耳机图标设计为 AirPods Max}

- macOS 的图标默认由三部分组成：背景图、中心图和文本，三者有其一即可。这些元素被放在一个右上角带有折痕的纸张上。最低可至 16*16 px @1x，那个时候就要缩减一些元素；

![1670057990525.png](Scenes%20Weekly%20%2362.assets/1670057990525.png)

{上图：macOS 图标组成部分}

- HIG 给我的感觉是，图标占比间距一直很乱、异形的图标也直接按照实际尺寸使用。而上面的 macOS 中心图则建议带有 10% 内间距的「出血」。实际上依然可以超过参考线对齐使用，详见本节最上方的视觉对齐。

![1670057991818.png](Scenes%20Weekly%20%2362.assets/1670057991818.png)

{上图：256*256 宽的区域内，留有 10% 内间距，心形图标的位置}

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/foundations/icons)

---

# 摘录

这周看过的一些——

> Controversial take incoming: STEAM REVIEWS DON'T REFLECT QUALITY. Rather they reflect matched player expectations, i.e. how much your actual game matches your steam store page marketing. I feel lots of game devs are not fully grasping this.

—— Riad Djemili [出处](https://twitter.com/riadd/status/1526505134133497858)

---

# 小事

1、目前的数字键盘不知你是否注意过，会分为两种：

![1670057992750.png](Scenes%20Weekly%20%2362.assets/1670057992750.png)

{上图：从上到下从左到右排列，左边是123456789*0#，右边是7894561230.=}

一般情况下左边是拨号，右边是计算器，为什么会有这么微妙的差异，两者区别在哪里？[DOC](https://www.doc.cc/about) 介绍了数字键盘历史，从 Jean-Baptiste Schwilguć 加法机的并排键盘到 Sundstrand 加法机带上数字 0 的 3x3+1 布局，从贝尔公司的 2x5 拨号按钮布局到 AT&T 筛选的 3x3+1 布局，虽说有专利避让原因，但也无法证明从上到下从左到右按顺序排列是最不容易操作失误的，[Keyboard Trivia](https://web.archive.org/web/20211004164540/http://www.vcalc.net/keyboard.htm) 有更详细的两个键盘布局对比总结，但依然没有定论。

→ [原文](https://www.doc.cc/articles/a-brief-history-of-the-numeric-keypad)

---

2、 Monotype 和新兴 web3 社区 KnownUnknown 云集了众多知名设计师联合创作了 Helvetica The NFT。按照官方的说法，该 NFT 系列旨在探索虚拟现实环境中的设计，虽然综合看来个别作品在「努力保留」瑞士主义风格，但是大部分作品依然融入 web3 式资本语言，这种杂糅看起来并不是那么舒适，或许 Helvetica 的固有印象已深入人心。

![1670057993662.jpeg](Scenes%20Weekly%20%2362.assets/1670057993662.jpeg)

{上图：Helvetica the NFT: Ben Jones (Copyright © Ben Jones, 2022)}

→ [网站](https://helvetica.knownunknown.com/)

---

3、PowerGlitch 是一个制作故障效果的网页小工具，可以调节时间、抖动和切片属性。

![1670057994664.gif](Scenes%20Weekly%20%2362.assets/1670057994664.gif)

{上图：本通讯标识测试 glitch 效果}

→ [网站](https://7ph.github.io/powerglitch/)

---

4、上周有一篇在 HN 上讨论度很高的文章，主人公 Michael Lynch 经营着一个 45,000 美元的项目，并想要重新设计他的产品网站。他预想的是仅重新设计首页、产品结算和购物车三个页面，预计花费 4 周 7000 美元左右，然而事实上花费了 8 个月 46,000 美元。

首先是 Lynch 主动找上了某设计供应商，这里化名为 WebAgency（Lynch 也太善良了）。Kick-off 会议后，WebAgency 赢得了 Lynch 的信任，为他规划了改版路线。先从标识重设计开始，需要 2-4 周（30-40 小时），时薪 175 美元。对接的客户经理 Isaac 解释道，WebAgency 还有签订长期合同的客户，会以他们需求优先。

他们现在 6 周内敲定了 TinyPilot 新标识改版方向，随后 WebAgency 向 Lynch 展示网站重设计的方向。

![1670057995893.png](Scenes%20Weekly%20%2362.assets/1670057995893.png)

{上图：WebAgency 提供的设计方向参考}

三个月过去了，WebAgency 的设计师继续在重新设计网站界面，之前设计的新标识反而置之不顾，连 Lynch 的小小修改需求都没有时间修改（agency 方说法）。当 WebAgency 展示重设计后网站时，Lynch 感到很诧异，之前说好的只需要重设计三个页面呢？客户经理 Isaac 又解释道，他们的首席设计师「对新项目感到非常兴奋，一不小心做过头了」，多出的工时不计入收费。

到了 12 月，项目进展几乎停滞。Lynch 以为是放假原因就没有催更。新年后工作节奏明显比之前慢了下来，质量也下降，自己的设计反馈也得不到回应。

2 月，Lynch 才问起 Isaac 怎么回事。对方答道，WebAgency 有项目经理辞职，人手不足，内部比较混乱。Lynch 是他们唯一的「小型客户」，除非签订每月 40 小时的合同才会提高优先级。受沉没成本桎梏，Lynch 继续与对方协商，Issac 也表示可以调整 12 月和 1 月工时退还差额，同时建议由 WebAgency 接手开发工作。

一环接一环下来，不知道 Lynch 还对这个 WebAgency 有多少耐心，但是顾及到自家开发人员使用 Python 和 JavaScript 较多，WebAgency 那边对复杂的 CSS 效果设计更有经验，即便价格依然昂贵，但还是同意了对方要求，为期 60 小时的工时合同。

接下来第一周 WebAgency 完成了剩余的设计任务，之后又是两周没有回应。Isaac 回复说 WebAgency 日程安排比较自由，并保证月底完成。然而到月底时，WebAgency 的开发只提交了一个小错误修复。4 月来了，对面开发又花了 5 周时间更换了 Bootstrap 主题。不是耸人听闻，其实是——

![1670057996820.png](Scenes%20Weekly%20%2362.assets/1670057996820.png)

{上图：花了 5 周时间和 6.1k 美元成本的前后页面对比}

5 月，Lynch 终于告知对方要解除合同了（提前 28 天），WebAgency 反而开发顺利。最后在 6 月，也就是合同到期后的第二天，项目终于交付完成。至于设计成果，任何设计师看到[这种界面](https://mtlynch.io/tinypilot-redesign/#before-and-after) 联系到如此高昂的报价都会直呼一声好家伙。

事后他们开了个电话会议，Issac 觉得这个项目很不顺利的原因是，WebAgency 难以缩小他们的流程以适应 Lynch 的预算。当 Lynch 提到想要看看项目维护日程表时，Issac 觉得成本有限就不做项目日程表了。

这个想想有些离谱，实际确实离谱的故事结局是，7 月份销售额比重设计前高出 66%。虽然在局外人看来这个网站重设计基本就是负优化，取消掉了实物展示，换以不明的插画，首页也没有说明白产品最基本的原理…… 但却得到了正面销售回报，这很可能是其他营销因素的成果。Lynch 对此还算满意。

原文结尾还列出了吸取的教训经验以及 FAQ。这也是 Michael Lynch 成为独立开发者后最擅长的事，4 年前他从 Google 离职后走了很多弯路，这次事件对于事业起色的他来说，也算是个性价比极高的免费营销。

→ [原文](https://mtlynch.io/tinypilot-redesign/)

---

> 我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 1 个订阅。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

→ [封面存档](https://figma.fun/f9e6Lk) ([figma.com](http://figma.com))

---

# 劳逸

![1670057997762.png](Scenes%20Weekly%20%2362.assets/1670057997762.png)

{上图：Stray 游戏 banner}

我把 Stray 这部游戏玩给我家猫看看，它感叹道里面的猫怎么体力这么好，是在哪里上蹿下跳的？我告诉它这是主角是一条走散的流浪猫，在一个赛博废土的世界里踏上归家之途。接着让它评价下里面猫的真实性，它告诉我步伐还不错，特别是下跳低处时先伸前爪很细节。一些独有的猫型互动让它直呼「演的吧」，我回道这不是和你日常一样。它没有否认，继续观察并说道，整体动作还是有些僵硬。说完便跑到一边继续趴着睡觉了。

我也退出了游戏，玩一段时间就会有晕 3D 的症状。因为 Stray 的交互很简单，跳跃也全靠视角操控，在定睛寻找目标时就会有所不适。解谜依赖试错，好在流程不长。

→ [获取游戏](https://store.steampowered.com/app/1332010/Stray/)

---

# 映像

现实拟像放映——

![1670057998953.jpeg](Scenes%20Weekly%20%2362.assets/1670057998953.jpeg)

{上图：Claes Oldenburg 雕塑：黄柄棕红相间的短扫把正在向蓝色的簸箕扫入纸团}

Big Sweep at the Denver Art Museum, Colorado

Photograph: robertharding/Alamy

---

# 温故

→ Scenes Weekly #13

[Scenes Weekly | No. 13](https://mp.weixin.qq.com/s/Q37AwaEC9ZtPXEwAM1ypvQ)

- 小镇设计
- Robinhood S-1 文件解析
- NSDockTile 案例
- A11y 指南 Access Guide
- 为什么一些高级设计师没有 portfolio 网站
- Big Mail 和 Meco 对比
- 实验网页设计思考
- Tesla FSD 镜头成像
- FBI 的蜜罐系统

---

喜欢本文的话，欢迎分享、订阅。

第 61 期请[在此查看](./Scenes Weekly #61.md)。

本次封面使用了 Public Sans 字体，灵感来源于家猫仰卧姿势。