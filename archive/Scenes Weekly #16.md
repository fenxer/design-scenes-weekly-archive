# Scenes Weekly #16

本系列为微博 @Design_Scenes 的每周总结以及其他杂事。

本周出现：GameStop、Signal、Safari、Steam、天气应用、Happy Hues、Live Text、React、Github、Behance、Discord、麦当劳、Screenly、Chartr、远程工作报告、TikTok、Kimono Project

---

# **周一**

上周的 **built for mars** 分享了一次 **Gamestop** 在线购物经历。问题主要为四点：

- Cookie 提示很大，取消流程很长；
- 图片渲染分辨率不对，有的地方没有 2x 优化。内容团队还有优化空间；
- 没有预测准确用户行为，很难帮用户找到TA们想要的商品；
- 加载时间长，页面优化差，加载时没有诸如 lazy load 等优化；

![640.jpeg](Scenes%20Weekly%20%2316.assets/640.jpeg)

起码现在来看，GS 转型后的电商体验依然不及 Amazon。

原链接 ↓

[A UX case study on Gamestop ✌️](https://builtformars.com/case-studies/can-gamestop-beat-amazon)

---

# **周三**

**Signal** 目前主要的「续航」手段依然是个人和组织的捐赠，但 app 上的捐赠体验在 **growth.design** 看来并不太友好。

下图在说明，原本底部的位置通常是广告等很容易被忽略的信息。如果真的想引起用户注意，还是应该置顶；另外文案也过于煽情性空洞，没有明确说出捐款的目的。

![640 (1).jpeg](Scenes%20Weekly%20%2316.assets/640%20(1).jpeg)

图二里，同样把捐赠一事感性化（插图和文字），真正重要的捐赠原因却在最底部；同时界面上给予用户过多的捐赠选择，不但没有必要，还产生了选择困难。

![640 (2).jpeg](Scenes%20Weekly%20%2316.assets/640%20(2).jpeg)

下图是捐赠完毕的界面，原版显得很应付，Louis-Xavier 的改版让它多了点人情味。这点上，buy me a coffee 做的就不错。

![640 (3).jpeg](Scenes%20Weekly%20%2316.assets/640%20(3).jpeg)

原链接 ↓

[Signal: How To Ethically Boost Your Revenues](https://growth.design/case-studies/signal-revenue/)

---

上周提到 Safari 的小改动：

> 长按地址栏也可以直接选择刷新，不用点三个点菜单（右一）。适用于滑到了页面底部时，无法触发在网页顶部的刷新机制。

> fenx，公众号：Design Scenes[Scenes Weekly | No. 15](./Scenes Weekly #15.md)

这周更新 beta 4 后，终于把刷新拿到最外层级了（长按菜单里也不再出现刷新）。

![640 (4).jpeg](Scenes%20Weekly%20%2316.assets/640%20(4).jpeg)

---

# **周四**

Steam 最近更新了移动端游戏详情页的界面。此前都是桌面端网页的响应式版本，各种选择器交互非常杂乱。新的界面更适合移动端浏览，不再有展开的侧边栏，并对多出的信息展示进行了折叠。

![640.png](Scenes%20Weekly%20%2316.assets/640.png)

但所谓的优化只是针对之前的界面，当前新的界面里一些字号和信息比重依然有很大的调整空间。

---

# **杂事**

1、因为摄氏度到华氏度的换算和四舍五入问题，iOS 某些版本（包括 iOS15 beta）的天气应用永远不会显示 69 华氏度。有人猜测 20°C = 68°F 21°C = 69.8°F，苹果不知何时引入了这种四舍五入导致了这个奇怪的问题。

The Verge 的报道 ↓

[Apple’s weather app won’t say it’s 69 degrees](https://www.theverge.com/tldr/2021/7/13/22575368/apple-ios-14-weather-app-69-rounding-error-15)

---

2、为网站寻找调色灵感时可以试试 **Happy Hues** ↓

![640 (1).png](Scenes%20Weekly%20%2316.assets/640%20(1).png)

[Happy Hues - Curated colors in context.](https://www.happyhues.co/)

---

**3、macOS Monterey Beta 4** 中，Live Text 向 Intel 设备开放。估计之前一直在为老机型做优化。

---

4、@oleg008 发推说自己做为前端设计师加入了特斯拉，来构造次世代的汽车生产流程用户界面。是的，他们用 **React**。

---

5、Github 最近增加了 **Cite** 仓库的小功能：

![640 (2).png](Scenes%20Weekly%20%2316.assets/640%20(2).png)

两种引用格式。前提需要 push **CITATION.cff** 文件到仓库根目录下。

---

**6、Behance** 对少数创作者开启了**订阅功能**（beta阶段），每月花费几美元可以解锁该创作者的源文件、额外收费的直播和付费项目。

![640 (3).png](Scenes%20Weekly%20%2316.assets/640%20(3).png)

不难理解 Behance 此举。甚至显得有些为时过晚。

详情说明 ↓

[25+ Creatives to Subscribe to on Behance](https://medium.com/behance-blog/25-creatives-to-subscribe-to-on-behance-4fc02fb3e8ee)

---

**7、Discord** 推出 Thread 功能，意在解决群对话中，前后文语境过长（插不上话）和多主题聊天（信息混乱）的问题。

![AnimatedImage.gif](Scenes%20Weekly%20%2316.assets/AnimatedImage.gif)

Thread 有最长可达一周的时间限制（分 Servers 等级），结束后可归档。可以选择创建公共还是私有的主题。

官方博客 ↓

[Connect the Conversation with Threads on Discord](https://blog.discord.com/connect-the-conversation-with-threads-on-discord-3f5fa8b0f6b)

之前我也分享过 Jarren 的一篇文章 → **The Future of Group Messaging**，他认为应该从群组信息的性质入手，去进一步划分信息应该存在的状态。比如 quote 一条对话，那么是不是代表接下来可以提炼出这些信息单独作为一个 “content” 区域，这个（临时的）话题只在这个区域里进行。这一切重点在于对信息内容和群聊交互的本质进行挖掘 ↓

[https://thejarren.com/group-messaging/](https://thejarren.com/group-messaging/)

Discord 是直接从主观上新建对话分支，和 Jarren 的 post 有异曲同工之处，但这类功能的诞生实际都以恰当使用为前提，警戒滥用才是难题。

---

**8、澳大利亚麦当劳**为了庆祝 50 周年，推出了 50 款限量 PS5 手柄，只有看了官方指定的直播才有机会得到：

![640 (4).png](Scenes%20Weekly%20%2316.assets/640%20(4).png)

红白黄的设计还挺耐看的（并不是每个人都是这种想法），但后来官方宣布推迟了活动举办，因为索尼那边没有授权……说不定转而送出其他奖品。

新闻详情 ↓

[The McDonalds Stream Week Has Been Postponed With New Prizing Confirmed](https://press-start.com.au/news/playstation/2021/07/31/mcdonalds-has-created-a-limited-edition-ps5-controller-that-aussies-can-win/)

---

9. 七月份 HN 上最激烈的开发者们讨论话题之一便是 **Safari** 的「罪与罚」，最新文章 ↓

Safari isn't protecting the web, it's killing it

[Safari isn't protecting the web, it's killing it](https://httptoolkit.tech/blog/safari-is-killing-the-web/)

但该文同样在 HN 上遭到不少反驳 ，有时间的可以去观摩一下大家对 Chrome 的「积恨」（好像没什么不对）。

---

**10、Screenly** 是一款给网页图片一键套上 mockup 的网页应用，支持自定义背景颜色和窗口样式（只有 macOS 样式）。自带的图片编辑也挺好用的。

![640 (5).png](Scenes%20Weekly%20%2316.assets/640%20(5).png)

适合非设计以及懒得动手的设计人员 ↓

[Screely - Generate Website Mockups](https://www.screely.com/)

---

**11、Chartr** 是我今天刚订阅的一个 newsletter，谢谢 The Sample 的推送。下图是根据苹果Q2财报整理的一份桑基图。

![640 (6).png](Scenes%20Weekly%20%2316.assets/640%20(6).png)

可以看到服务型产品收益毛利率很高，这依赖于苹果产品的生态建设。

本期地址 ↓

[https://www.chartr.co/newsletters/2021/7/28/how-apple-makes-its-money](https://www.chartr.co/newsletters/2021/7/28/how-apple-makes-its-money)

---

**12、CraftJack** 的一项研究发现，45%的远程工作者在沙发上工作，**38%在床上**。这两种习惯其实都对身体很不好，花几千甚至几万投资一套符合人体工程桌椅还是有必要的。

---

13、华尔街日报搞了 100 个机器人，分别带上不同的属性标签，去刷 **tiktok** 看它的算法能否识别出机器人的用户属性，结果最长只需200多个视频 tiktok 就摸透了。当然这个视频只是讲算法的应用原理而不是算法本身，请了前 Youtube 算法专家（现专注于算法透明）过来也只是浅尝辄止。

视频 ↓

[How TikTok's Algorithm Figures You Out | WSJ](https://www.youtube.com/watch?v=nfczi2cI6Cs)

---

14. **KIMONO Project**，一个触及全球 207 个国家和地区的和服设计计划。

中国样式为：

![640 (7).png](Scenes%20Weekly%20%2316.assets/640%20(7).png)

涵盖了龙、长城、牡丹、竹、云、水墨画风格的山河线条以及熊猫。带子（Obi）则以唐三彩为灵感元素。

---

封面使用了 Anderson Grotesk 字体。