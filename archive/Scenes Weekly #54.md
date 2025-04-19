# Scenes Weekly #54

2022-05-16

\> 设计视角下的世界——

第 53 期请[在此查看](./Scenes Weekly #53.md)。

本期出现：

- Figma Config 2022 观后感
- PPT 新玩具 Weavve
- Google I/O 中的 Monk Skin Tone Scale
- Massimo Vignelli 诞辰 90 周年纪念（2021）
- 其他：React.js logo、Cursor Dance Party

如有格式异常建议点击最上方「在浏览器中访问」。

---

# 杂事

1、今年 Figma Config 2022 一样带来很多新改进，与去年 FigJam 业务拓展不同，今年的改变更专注于基础功能维护。

首先是千呼万唤的暗色主题终于实装，在这之前无论是第三方插件还是愚人节笑话我们都窥到了 Figma 暗色的一面，所以有一种惊喜了又没惊喜的感觉。Figma 官方的暗色主题并没有改变画布背景（这是合理的），我自己的话一般使用 # 1A1A1A 作为暗色画布，设计内容区域比周围更暗一点，也是从 Sketch 下来的视觉习惯。

Figma 的暗示模式并没有太惊艳的感觉，反而觉得有一丝杂乱。比如分割线条太多，亮度不低；某些区域信息密度高导致暗底白色看的很累等等。目前一些插件的背景还没有适配自适应主题（没使用到他们的 color tokens）。在 Config 2022 上，Ryhan Hassan 和 Jacob Miller 分享了搭建暗色模式设计系统中颜色的升级，Ryhan 在自己的 Twitter 上[也有提及](https://twitter.com/ryhanhassan/status/1524055454929670145)。需要说明的是，新设计都要有一个熟悉的过程，这只是第一印象。

随之还有可变字体的支持。六年了，之后安装字体终于可以不用选择静态字体。同时文本支持单行超出内容截断为省略号 … 显示，也是一个相当实用的功能。不同的是，前者计入字体样式（Type Styles），后者则是独立的设置。另外可变字体的调节轴给出了默认值和节点标识，优化到位。

![1669798189449.png](Scenes%20Weekly%20%2354.assets/1669798189449.png)

{上图：文本截断和可变字体功能}

Auto Layout 重新布局了各个选项设置，Alignment 不用在小弹框里设置，Resizing 也不必和 Constraints 挤在一起。还增加了对描边在间距中的处理、负间距时图层堆叠顺序、基线对齐等选项。以及「致命一击的」绝对定位（Absolute positioning）功能，都更加贴近了前端流动布局逻辑，早这样多好。

Variant 功能撑起了绝大部分 Design System 的实用性，新推出的 Component properties 可以大幅度减少一个组件的变体数量，转换为组件属性去管理。比如一个组件中的图标替换、文本更改、元素是否显示都不必再用变体展示，两者相辅相成。

![1669798191163.png](Scenes%20Weekly%20%2354.assets/1669798191163.png)

{上图：变体属性和组件属性的对比}

两者都有 Playground 文件体验。

另外还有：

- 原型里的动画更新了弹性曲率，默认提供四个值，并且可自定义。试用体验很不错。
- 描边支持四条边独立设置粗细，但依然无法独立设置颜色，不过这已经对列表布局起到很大作用；
- Spotlight 功能可以让所有协作人员的屏幕都以自己的为准，不用让每个人都去掉自己头像；
- 文件链接现在可以带上密码分享，但不支持免费个人版；
- FigJam 新的 Jira、Asanaand 和 GitHub widgets 跟踪 issues，以及创建贺卡和语音备忘的 widgets；
- Widget Code Generator 可以使用 Figma 直接设计并生成 widget 代码；
- 基于其他键盘布局的快捷键显示；
- 新的 Show Outlines 可以显示隐藏图层的框架（很有用）；

→ 查看所有更新

[What's New in Figma](https://www.figma.com/whats-new/)

另外 Figma Community Awards 结果也出炉了，[详见](https://www.figma.com/blog/figma-community-awards-2022/)。

目前社区还比较乱，没有一个固定的地方能找到所有 Config 2022 演示文稿。

---

2、从 Google Slides 到 Pitch，PPT「制作降级」不断推进。可惜只要是带有一定目的性的 PPT，不论多易用多有趣也会感到疲惫。Weavve 这款新产品也是打算让 PPT 变得 "the joyful and easy-to-use"，不考虑个人情绪，它的交互勾起了我的兴趣。

![1669798195896.png](Scenes%20Weekly%20%2354.assets/1669798195896.png)

{上图：Weavve 界面预览}

目前官网只能找到这一张预览图，网格导向的排版首先想起了 [Universe](https://onuniverse.com/) 那款建站应用。但 Universe 是基于移动端体验优先的，在有着更多选择的桌面端上，[Readymag](https://readymag.com/) 是对标的好对象之一。Weavve 作为 PPT 工具虽然没有必要构造那么复杂的编辑器，但我依然希望能看到 Readymag 一样的优雅。

Weavve 在四月发出了第一波邀请使用资格，没赶上，等待后续详细体验机会。

→ 官网

[weavve • The joyful alternative to Powerpoint and Google Slides](https://www.weavve.io/)

---

3、今年的 Google I/O 大会稍有些平淡，就像提到 RCS 时的现场观众一样冷清（[第 39 期](https://designscenes.zhubai.love/posts/2094753654367477760#:~:text=%E8%93%9D%E7%BB%BF%E6%B0%94%E6%B3%A1%E8%A7%A3%E9%87%8A%7D-,Google%20%E6%83%B3%E8%A6%81%E6%8E%A8%E5%8A%A8%20RCS,-%EF%BC%88%E8%9E%8D%E5%90%88%E9%80%9A%E4%BF%A1%EF%BC%89%E4%B8%9A%E5%8A%A1)提到 Google 想要推动 RCS 标准）。Pixel 6a 还是等买的话再说，其他有兴趣的应该就是 Monk 肤色量表了。变相回答了很久之前自学手绘时对肤色色值的疑问。

该量表希望作为一种肤色测量标准，改善 AI 中的一些偏见训练以及产品中的一些多样性问题，比如 emoji 的肤色选择（？）之前 [Fitzpatrick scale](https://en.wikipedia.org/wiki/Fitzpatrick_scale) 5 种肤色类型饱受争议，Google 将其拓展为 10 种，而又不像美妆行业动辄 40+ 色调那么复杂。

![1669798197709.png](Scenes%20Weekly%20%2354.assets/1669798197709.png)

{上图：十种肤色的颜色 Hex 值}

同时 Google 提醒道，实际图片中的肤色可能会受环境影响，一个人对肤色的判断也是主观的。最重要的是，不要将肤色与种族挂钩，原本社会学家 Monk 博士就为了将次两者相区分才开发的此量表标准。

Google 未来将把此量表加入相册和图片搜索的筛选中。

→ Skin Tone Research @ Google AI

[Skin Tone Research @ Google](https://skintone.google/)

---

4、

> If you can design one thing, you can design everything.

如此感人的话语可能只有从设计同行口中才能说出来。去年 2021 年是信息设计师 Massimo Vignelli 诞辰 90 周年，Vignelli90 这个网站展示了来自全球 46 个国家的设计师的 252 封海报，以纪念这位跨领域的设计大师。虽说里面繁多的设计都是缅怀之情，但其设计本身也有很多参考借鉴的意义。

→ Vignelli90

[https://www.vignelli.design/](https://www.vignelli.design/)

---

5、Maykel 分享了他在 2013 年为准备开源的 React.js 绘制 logo 时的灵感来源，FedEx 的设计太经典了。

![1669798199505.png](Scenes%20Weekly%20%2354.assets/1669798199505.png)

{上图：React logo}

先是在草图上画了简单的原子形状，然后中间加了圆，负空间像一个代表工程、开发和工具等 mood 的齿轮。于是敲定了这个标识。

→ 原文

[How FedEx Influenced the React Logo — Maykel Loomans](https://maykelloomans.com/notebook/how-fedex-influenced-the-react-logo)

---

6、Cursor Dance Party 这个网页和 [Cursor Disco](https://cursordisco.ytmnd.com/) 一样经典，可以变换鼠标形态，然后一起 party——

![1669798202730.png](Scenes%20Weekly%20%2354.assets/1669798202730.png)

{上图：Cursor Dance Party 网页截图}

这个有趣的网页上次在 HN 出现已是十年前，最近又被发出来然后把服务器流量额度用光了…… 目前处于不可访问状态。

→ 网站

[Cursor Dance Party!](https://www.cursordanceparty.com/)

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周更新了 2 个。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

---

# 摘录

这周看过的一些——

> Put simply, metaverses turn digital serfs into homesteaders.

—— 7 Essential Ingredients of a Metaverse | Future

[7 Essential Ingredients of a Metaverse](https://future.a16z.com/7-essential-ingredients-of-a-metaverse/)

---

# 劳逸

![1669798204634.png](Scenes%20Weekly%20%2354.assets/1669798204634.png)

{上图：FFO 游戏截图}

在两度对地平线 2 西之绝境 提不起兴趣后，我居然在一周内打通了最终幻想起源（后简称 FFO），时间没超过 30 小时。FFO 和地平线 2 可谓是对比鲜明，前者除了 Team Ninja 打造的多职业动作系统外一无是处（特别是画质），后者除了次时代画质外也一无可取（特别是战斗）。

除了最终幻想系列大量的职业组合之外，在科技与魔法的表象背后还有着系列传承的主题，即角色们通过冒险，一步步走上反叛、摆脱命运掌控的道路。FFO 的故事也是如此，奈何在 Team Ninja 的手中，叙事变得极为糟糕，几乎在明说「Square Enix 没给够预算」。总的来说故事本身不错，搭配忍龙、仁王一样的流畅战斗，对最终幻想粉丝来说还是值得一玩的。

→ 游戏获取（也有 PS 平台）

[STRANGER OF PARADISE FINAL FANTASY ORIGIN | Download and Buy Today - Epic Games Store](https://store.epicgames.com/en-US/p/stranger-of-paradise-final-fantasy-origin)

---

# 映像

现实拟像放映——

![1669798206365.jpeg](Scenes%20Weekly%20%2354.assets/1669798206365.jpeg)

{上图：楼宇中密集的阳台被蓝紫黄绿粉等颜色覆盖}

© Michael Wolf

Life in cities - architecture of density

---

# 温故

→ Scenes Weekly #5

[Scenes Weekly | No. 5](https://mp.weixin.qq.com/s/fN6F9fImL_ghrVYOX6SiMA)

- Dashword 应用重新组织了笔记中 list 样式
- figma.fun 可以把冗长的 Figma 分享链接转变为短链接
- Windows Vista 开发时期一些神奇的设计示例
- Daniel Eden 个人网站 9 年历经 20 次改版
- 在线杂志 Tablet 交互鉴赏

---

喜欢本文的话，欢迎分享、订阅。

第 53 期请[在此查看](./Scenes Weekly #53.md)。

本次封面使用了 Cabinet Grotesk 字体。

