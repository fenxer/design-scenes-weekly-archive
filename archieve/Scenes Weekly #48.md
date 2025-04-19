# Scenes Weekly #48

2022-04-06

\> 设计视角下的世界——

第 47 期请[在此查看](./Scenes Weekly #47.md)。

本期出现：Firefox、Localization、Color Picker、Design Details、[x]it!、Coda CD、Chrome 100、Instagram Thread、68th TDC awards、The Chinese Type Archive、Tab Maker、Figma、Mac External Displays

如有格式异常建议点击最上方「在浏览器中访问」。

---

每月 4 期，在本期终于跑完了一年这一圈。以后大概我也可以加上 "Revisit" 栏目了。

本通讯原本是为了不让「稍后再看」变成「再也不看」，从第一年的微博实时记录，也转换到现在更适合自己的 newsletter 形式。至于一直没有见涨的订阅数，就像之前看到别人说的那样，当你的写作没有超出观众的期待，虽然不会掉粉，但也基本无法形成传播。作为一名还在一线的打工人，能在每周拿出8小时左右时间去维护自己的好奇心，已经有些濒临上限了。当然自己在各方面的能力也还有大量提升的空间，希望下一个四十八*，你我都能有新的一面。

- 每年有52周，剩下 4 周想留给休假等一些意外事项。去年一年共休息 2 期，所以严谨地说，第50期才是完整的第一年。

---

# 摘录

这周看过的一些——

> 按照维特根斯坦的观点，哲学在于给出「阐释」，而不在于提出《逻辑哲学论》所讲的「命题」，这当然是对的；但是读者也许有理由认为如果使用的最重要概念——如「名称」和「客体」——没有得到解释的话，那就什么也没有阐明，所以他还是不了解怎样使用它们；……

> 关于语言及其与世界之映示关系的论题，所得出的结论是一旦我们从结构问题中抽身，开始转而弄清学说的实际意思（用维特根斯坦的话讲就是“正确地看世界”）时，整个方案便证明是行不通的：因为人们确确实实不知道维特根斯坦自己在讲些什么。

—— A·C·格雷林 -《维特根斯坦与哲学》

---

# 杂事

1、自Firefox 舍弃 Photon 换用 Proton 后，后者一直在用户群体中争议不断。但得益于 Firefox 的高度定制化，诞生了Lepton 这么一个用户自发去完善 Proton 的开源项目。在项目的 wiki 页面，有一篇介绍 Firefox 浏览器界面历史的文章。

![141683937-ae564033-fbb8-4b7a-9fff-4b3fe3fd388b.png](Scenes%20Weekly%20%2348.assets/141683937-ae564033-fbb8-4b7a-9fff-4b3fe3fd388b.png)

{上图：Firefox 2002年的版本}

想起自己作为 Firefox 的日常用户还是十几年前的学生时期，接触最多的界面应该是v3 和 v4 版本 Classic theme，对缓缓出现的右侧小地址栏还留有印象。后面的 Australis 版本发布时，我早已投奔 Chrome，但”fast and soft” 理念看起来确实很和谐。后来想看看 Firefox 发展如何时，又被 Win10 时代的 Photon 过于繁重和乏味的界面劝退，即便[看起来大家](https://news.ycombinator.com/item?id=30820894)都挺喜欢 Photon。

![73e422b3a22529a3d97c07d4bf41461b.png](Scenes%20Weekly%20%2348.assets/73e422b3a22529a3d97c07d4bf41461b.png)

{上图：Lepton 右键改进}

直到我看到了上图，本来对系统原生空间的摒弃已经一种不可逆的趋势，但 Proton 这个 mac 右键菜单确实过分了一点……

原文依次列举了每个阶段界面的优缺点，还有一些热力图分析（官方数据），值得参考。

→ 原文

[[Article] 0. Firefox UI UX history · black7375/Firefox-UI-Fix Wiki](https://github.com/black7375/Firefox-UI-Fix/wiki/%5BArticle%5D-0.-Firefox-UI-UX-history)

---

2、网站语言/地区切换的几个tips：

- 默认匹配用户当前环境语言。除了网站，很多应用也是匹配系统地区和语言。
- 无法匹配的话可以单独在流程中插入语言/地区选择。但是个人觉得如非重要不必打断用户浏览进度。
- 一般切换选择器都会放置在右上角，配合语言/地区图标和**当前语言**显示的名称。
- 语言列表中，使用当地语言显示可以让用户更快地找到所需。比如从英文切换到中文，语言列表中最好显示「简体中文」而不是 “Simplified Chinese”。
- 要注意一些地区和语言的多样性组合。比如原文中提到，印度的电商行业中，印度购物者更喜欢在英文网站上购物而不是印度语。

→ 原文

[6 Tips for Improving Language Switchers on Ecommerce Sites](https://www.nngroup.com/articles/language-switching-ecommerce/)

---

3、@dustin 分享了 The Browser Company 产品中的颜色选择器设计思路。

![AnimatedImage.gif](Scenes%20Weekly%20%2348.assets/AnimatedImage.gif)

{上图：选择器演示}

传统的颜色选择器是基于精确性打造的，过于理性。@dustin 和团队的人从一些音乐应用的设置里得到灵感，想让颜色选择器更加感性化和人性化。总结下来三点便是：

- 强调探索；
- 隐藏复杂的机制（RGB条选色实在太反人类了）；
- 所见即所得；

这三者结合起来是带有一定飞轮特性的，只有让选色变得直觉化，才会引起用户探索使用的欲望，探索的结果即时得到反馈也更符合人性直觉。

→ 详见原推

[登录 Twitter，关注dustin senos](https://twitter.com/dustin/status/1508500466505699331)

---

4、讲述设计细节的文章不计其数，David Hoang 这篇文章也总结了一些好的设计所具备的要素：

- 预测性；
- 循序渐进解决问题；
- 一定的美学；
- 捷径；
- 「过于聪明」；
- 考虑人与场景；

这些要素我们可能听过太多次了，所以不如直接看看下面的案例。第一个提到的是 Vercel 的网站 logo 细节，当你右键 logo 时会自动跳到 Vercel 的品牌指导页面，并且第一个按钮就是提供品牌标识下载。

![vercel.jpeg](Scenes%20Weekly%20%2348.assets/vercel.jpeg)

{上图：Vercel Design 页面}

最后 Hoang 提到了 Command Palette 这个设计模式（类似 macOS 的聚焦搜索）。我们能感知到近几年这个模式的流行，但是其背后隐藏着对快捷指令设计和改变用户习惯引导设计的高度要求，所以很佩服 Raycast 做出的各种探索。

→ 查看原文更多案例

[Snippets of good design](https://davidhoang.substack.com/p/snippets-of-good-design)

---

5、[x]it! 是一个纯文本 todo-list 格式，保存的 .xit 文件可被普通文档编辑器打开，同时支持 Sublime Text 和 VSCode 的插件来优化文本格式。

![截屏2022-04-03 16.01.49.png](Scenes%20Weekly%20%2348.assets/%E6%88%AA%E5%B1%8F2022-04-03%2016.01.49.png)

{上图：不同编辑器打开 .xit 文件对比}

支持四种状态、优先级（可用红点占位对齐）、日期格式、分组和标签功能，五脏俱全。比 markdown 还丰富一些。轻标记语言带来的纯文本开始有「复古思潮」的趋势。

→ 当然是开源的

[[x]it! – A plain-text file format for todos and check lists](https://xit.jotaen.net/)

---

6、苹果《健听女孩》DVD 拆箱体验。原本是为奥斯卡送审用的，所以原作者也收到了一份。

![coda.png](Scenes%20Weekly%20%2348.assets/coda.png)

{上图：蚀刻在反射层上的CODA标识，没有打印一层标签贴在上面}

→ An Apple Original on DVD: The Definitive Unboxing and UX Review

[An Apple Original on DVD: The Definitive Unboxing and UX Review](https://thenougatmachine.wordpress.com/2022/03/23/an-apple-original-on-dvd-the-definitive-unboxing-and-ux-review/)

---

7、值此 Chrome 正式版版本号 100 之际，Chrome 官方列出了自 2008 年以来互联网进化过程中一些很酷的事件。

→ 100 cool web moments

[#100CoolWebMoments - Chrome Developers](https://developer.chrome.com/100/)

---

8、之前写过 Instagram Threads [On Building a Fluid User Interface](https://about.instagram.com/blog/engineering/on-building-a-fluid-user-interface) 这篇文章的 Rishi Mody，披露了去年还在做 Threads 时，恶搞地做了一个 Win95 风格的界面。

![截屏2022-04-02 17.45.21.png](Scenes%20Weekly%20%2348.assets/%E6%88%AA%E5%B1%8F2022-04-02%2017.45.21.png)

{上图：Win95 风格 Threads}

早年 Petrick Animation 也做过一个类似的[概念设计](https://www.behance.net/gallery/41023081/Instagram-for-Win95)。

→ 原推

[登录 Twitter，关注Rishi Mody ツ](https://twitter.com/rishmody/status/1508793160301957121)

---

9、第68届纽约TDC 近300幅获奖作品公示。超过60个国家的22个品类，可谓是每年的年度平面设计盛宴。

→ 查看获奖作品

[https://www.oneclub.org/awards/tdcawards/-archive/awards/2022/all/all/select](https://www.oneclub.org/awards/tdcawards/-archive/awards/2022/all/all/select)

→ 三言也写了一篇关于获奖中文字体的

[https://mp.weixin.qq.com/s/BV4Bx5rZ7nj_N6f_7BLmuw](https://mp.weixin.qq.com/s/BV4Bx5rZ7nj_N6f_7BLmuw)

10、The Chinese Type Archive 是一个供全世界字体设计人士阅读参考的资料库。从中文字族到字体术语，再到一些中文字体设计书刊，图文并茂，资料非常丰富。只是很奇怪首页为什么是随机挑选的三个词条（好歹提示一下）……

![截屏2022-04-03 17.22.42.png](Scenes%20Weekly%20%2348.assets/%E6%88%AA%E5%B1%8F2022-04-03%2017.22.42.png)

{上图：中宫词条截取}

→ The Chinese Type Archive

[The Chinese Type Archive / 字體資料庫](https://chinesetypearchive.com/#/)

---

11、Tab Maker 是 Google Chrome Experiment 项目的一员，可以根据自己的喜好制作 NTP（新标签页）扩展。突出一个花里胡哨，但是数据的字段填充却用的是电子表格……很疑惑这种不「平民」的方式是不是为了 Google Sheet 宣传。

→ Tab Maker

[Tab Maker](https://tabmaker.withgoogle.com/)

---

12、之前提到过 Figma 本地化进度的怠惰，最近他们终于开始加速，先是设立日本办公室，而后开始支持 RTL 语言。值得注意的是原文最后一段：

> Figma is built to be an inclusive space where everyone is invited to design, build, and play. We understand that it’s 2022, and the world has a range of stereotypes about Americans, let alone American tech companies. As Figma enters new markets, we pledge to show up with humility and a learning mindset. There may be times when we miss the mark or when our efforts get lost in translation. My only ask: let us know when we mess up so we can learn and get better.

而且 [Our journey to Japan](https://www.figma.com/blog/expanding-figmas-international-presence/#our-journey-to-japan) 那一段所说的日本市场状况，我觉得国内也非常符合。但鉴于日本消费者对本土品牌有一种莫名的信任感，像是 Kakao、NHN 的手段屡试不爽，再加上国内对内容的审查，估计和 Figma 文化价值观有不少冲突……不难理解日本作为亚洲第一个本地化站点了。

→ Localization, languages, and listening

[Localization, languages, and listening](https://www.figma.com/blog/expanding-figmas-international-presence/)

---

13、bjango 的博客更新了 mac 外接设计向显示器推荐，[上一篇](https://bjango.com/articles/macexternaldisplays/)还是2016年，6年间对显示器而言，mac 适配显示器依然是小众需求。直至 Apple Studio Display 的出现，让原作者才有了更新这篇文章的想法。虚化的像素是 retina 的大敌，原文介绍了各 PPI 的直观对比。

→ Mac external displays for designers and developers, part 2

[Mac external displays for designers and developers, part 2](https://bjango.com/articles/macexternaldisplays2/)

---

# 劳逸

![AnimatedImage.gif](Scenes%20Weekly%20%2348.assets/AnimatedImage%20(2).gif)

{上图：A Short Hike 多人模式}

2019 年发售的广受好评的休闲冒险游戏 A Short Hike，其开发者 adamgryu 最近在 [itch.io](http://itch.io) 推出了实验性在线联机版，最高支持99人联机。现已在 Steam 的 beta 分支和其他平台推出， adamgryu 表示不会长期支持，但可以自己建立联机服务器。

→ mod 说明

[A Short Hike 99 - Online Multiplayer Mod by adamgryu](https://adamgryu.itch.io/a-short-hike-99-online-mod)

---

# 映像

现实拟像放映——

![8b2cd089ee5e440c8c6f52cdcb6b6a93.jpeg](Scenes%20Weekly%20%2348.assets/8b2cd089ee5e440c8c6f52cdcb6b6a93.jpeg)

{上图：Shape, Stamp, Stack.}

[@d.esk](https://d-esk.net/Shape-Stamp-Stack)

---

喜欢本文的话，欢迎分享、订阅。

第 47 期请[在此查看](./Scenes Weekly #47.md)。

本次封面使用了 Meshed Display 字体，tape 样式来自 Figma 2022 年愚人节。