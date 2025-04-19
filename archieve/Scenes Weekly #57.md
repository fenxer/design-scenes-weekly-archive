# Scenes Weekly #57

2022-06-13

\> 设计视角下的世界——

第 56 期请[在此查看](./Scenes Weekly #56.md)。

本期出现：

- WWDC 碎碎念
- Product Hunt 产品详情页面改版
- Human Interface Guidelines 更新
- Google Brain Team 的文字转图像 AI Imagen
- 古早教科书的插画鉴赏
- Arc 浏览器公布前瞻
- Don't Wordle 介绍
- 国内产品的无障碍改造艰辛探索之路
- 零知识证明小工具 zk-Crush
- 蒙娜丽莎又遭蛋糕袭击
- 其他：网页万花尺、美国外卖平台现状、Chineasy 应用、Notion 插件 Slashy、OpenSea 内幕交易、IINA 支持 HDR、Sketch 采访 Gavin Nelson、Figma 采访 Thierry Blancpain、Sliderland、AI 图片编辑工具 Depix、Know Your Meme 总编 Don Caldwell 采访、阿里健康体、纯文本插入图形元素

如有格式异常建议点击最上方「在浏览器中访问」。

---

上周因端午放假停更一期，积攒了不少信息。六月上半的展会很多，先简单写写过渡一下。

下周搬家，所以依然有可能停更（繁忙的六月）。

另外欢迎上两周的新订阅者们，感谢所有订阅者的支持。

---

# WWDC22 碎碎念

以下是对今年 WWDC 的吐槽，可跳过，正文在后面。

- 今年 WWDC22 的大部分功能依旧是跨平台的，然后分别在 iOS、iPadOS 和 macOS 中优先演示，这样代表了这些功能起源于何处、拓展于何方；
- **台前调度的左侧应用缩略图带有倾斜的角度，很有 RealityOS 影子；**
- Live Text 可以在视频帧中使用。并且支持了日语、韩语和乌克兰语。但实际测试还是有点傻傻分不清日语中的汉字，很大因素取决于系统语言…… 这点还不如很久都没更新的 Mac QQ 自带的 OCR。文本翻译的质量也仅仅处于能看的水平；

![1669971062758.png](Scenes%20Weekly%20%2357.assets/1669971062758.png)

{上图：某日服手游录屏，暂停视频后使用 Live Text 识别}

- 相册自带抠图真好用；
- 图书应用更新，菜单更符合现在 iOS 的设计风格，增加了调整行距、字距、词距选项。但是之前拟物翻页效果不见了，变为横移；
- 系统级的协作功能 API，感觉 Craig 轻描淡写地说出了 Apple 又一野心（另一个 CarPlay）；
- [第 55 期](https://designscenes.zhubai.love/posts/2140365736035151872)的摘录里，摘取了 Casper Kessels 评测保时捷 Taycan 时的一句话：

> "It amazes me that in the 8 years since Apple CarPlay and Android Auto were released, very few carmakers have built systems that can rival those running on our phones."

- 现在发力的 CarPlay 想要进一步拉开这个差距。联想到造车的 Apple，无论数据上还是营销上都不可小觑；
- 锁屏界面：
    - Apple 在 macOS 端买了那么多字体终于给 iOS 用上一些了；
    - 类似杂志封面的人物主体突出为整体增色不少，可以称得上是拿得出手的事情；
    - 但是 iPad 锁屏却不支持自定义，仅加粗了时间字体；
    - 让我想起以前 HTC 的 Sense 系统，只不过当年的金属圆环现在变为了横线；
- watchOS 9 大都会表盘（Metropolitan）又是一款优秀的可变字体实例，如下方动图演示，12 枚数字随着数码表冠变换了高度和宽度。

![1669971066876.gif](Scenes%20Weekly%20%2357.assets/1669971066876.gif)

{上图：大都会表盘的字体变换}

- 这种 type-driven 的表盘，去年秋季发布的 S7 就有体现（详见[第 23 期](https://mp.weixin.qq.com/s/trmup73B9Qw2MNgBiLmLIg)）；
- 睡眠应用终于没那么鸡肋了，可以记录睡眠阶段。但是在这之前为什么戴表睡觉的问题，对我来说没解决；
- 药理提示是个好功能，之前仅有一些第三方应用在做，希望能受到更多重视；
- 跑步的改动可以看 Wired 写的[一篇新闻](https://www.wired.com/story/apple-watch-watchos9-the-best-running-watch/)；
- macOS 13 起名为 Ventura，感到近几年的命名词汇音节越来越标准好记了。Venture 这个词早在库乐队教程中的一首歌就有出现，歌名为 Ventura Highway（via. [IT Media](https://www.itmedia.co.jp/news/articles/2206/07/news069_5.html)）;
    - 系统偏好设置界面大改，设计趋近 iPad。然后没把之前的半拟物图标带过来，不好；
    - Jeff Johnson 特意写了一篇文章，批判 Ventura 偏好界面的种种功能阉割；
- 图像引擎 Metal 也迎来了新的升级。最瞩目的是类似 DLSS 和 FSR 的 MetalFX Upscaling 技术，使用上采样结合 TAA 抗锯齿技术来运行一些吃性能的游戏。不过看生化危机 8 的演示画面感觉比较一般（没有风扇的 MBP Air 洗洗睡吧）；
    - 但目前 Metal 的优化大多面向的是玩家（Fast Resource Loading API 也是），开发 / 移植的难易程度依旧是 Apple 桌面端游戏生态的一大因素；
- M2 相关依然可以看 [Anand Tech 的总结](https://www.anandtech.com/show/17431/apple-announces-m2-soc-apple-silicon-updated-for-2022)；
- 苹果的数据图表一如既往的「极简」，还得多看文末注释；
    - 比如演示里 the latest 10-core PC laptop chip 指的是 Samsung Galaxy Book2 360 的 Core i7-1255U；
- 今年 5 月 5 日，Apple、Microsoft、Google 联合 FIDO 加快推进无密码技术标准的施行。去年 WWDC，Apple 推出了 passkeys in iCloud keychain 标准，今年落地，旨在替代密码，采用更多的生物识别，生成的 Passkey 端到端加密，只有你持有私钥；
    - 密码设置里可以集中第三方 2FA 应用；
- 一些苹果笑话：

![1669971071698.png](Scenes%20Weekly%20%2357.assets/1669971071698.png)

{上图：Apple 单卖的 USB-C to MagSafe 3 线与宣传图对照}

- 其他细节更新等自己体验到新系统再说吧，SF Symbols 4 也是个不小的吸引力；
- 不光 AR/VR 相关传闻落空，[有消息称](https://www.tweaktown.com/news/86518/apple-search-engine-rumored-siri-could-finally-get-smart/index.html) Apple 还会发布新的搜索引擎（更聪明的 Siri？）也没有公布；

---

# 摘录

这周看过的一些——

> The rules for luxury brands are very different from those for other kinds of retailers — mostly because the decision-making process for luxury purchases is not practical, but intensely emotional. Luxury marketing relies heavily on establishing and protecting a brand narrative — particularly around quality and exclusivity.

> Most retailers have a strong motivation to sell as many products to as many people as possible, but luxury brands must be wary of expansion. This is a matter of access as well as price — the more people that own the product, the less exclusive it is. These brands don’t want to sell to everyone — they want to sell to the “right” people. They exist to define social status. As a result, the rules for luxury sometimes blatantly violate usability. They want to make customers “work” to “earn” the product.

—— Kate Moran - [Why So Many Luxury Brands Are Terrible at Ecommerce](https://www.nngroup.com/articles/luxury-terrible-ecommerce/)

---

# 休闲一刻

1、Product Hunt 产品详情页面改版，一度让我以为页面的什么元素没加载出来。过多信息集中在正文附近，没有做明显区分。同时缩小了产品介绍图，增加两排头像展示参与此产品互动的用户。底部增加了产品的投票和排行信息。整体抛弃了原有卡片布局，比 Patreon 少了点线条。

![1669971076084.png](Scenes%20Weekly%20%2357.assets/1669971076084.png)

{上图：新版 Product Hunt 详情页截图}

---

2、我对图像管理应用 Eagle 最深的印象是…… 菜单中的【导出到计算机】——虽然用了多年 Eagle，但只能算浅度用户。目前还有 128 张图处于未标签状态，提不起劲，也不指望 Eagle 产品上能让我提起劲。所以这次 3.0 更新基本没什么想法。资源社区很杂，特别是一些设定集，游走在灰色边缘。上一个这么传设定集的网站是什么呢——e-hentai（NSFW⚠️）。

---

3、Apple 这次 WWDC 也更新了 Human Interface Guidelines，不光重新编排了目录，还增添了大量内容，应该是本次 WWDC 最大的惊喜。我还没有仔细重新阅读，但是看了下 [Right to left](https://developer.apple.com/design/human-interface-guidelines/foundations/right-to-left) 这章的详细度就能明白此次更新有多么丰富。如果我没在写 newsletter 现在一定在记笔记了。

→ 新 HIG

[Human Interface Guidelines - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/guidelines/overview)

---

4、 Nathan Friend 之前把童年玩具「万花尺」做成了 app，现在做了网页版 Inspiral web，用来生成 Spirograph Art。

![1669971077973.gif](Scenes%20Weekly%20%2357.assets/1669971077973.gif)

{上图：Inspiral web 试玩，正式中文名貌似叫繁花曲线规？}

网页版有 gallery 展示其他的创作。右侧有个细节是，铅笔的颜色貌似取自彩铅。

→ 体验

[Inspiral Web](https://nathanfriend.io/inspiral-web/)

---

5、美国外卖平台现状（Q1）：

![1669971081524.png](Scenes%20Weekly%20%2357.assets/1669971081524.png)

{上图：DoorDash 市场份额、人均消费、客单价曲线}

→ 来源

[DoorDash customer loyalty drives share gains - Earnest Analytics](https://www.earnestresearch.com/data-bites/doordash-customer-loyalty-drives-share-gains/)

---

6、Google Brain Team 也公布了基于扩散模型的文字转图像 AI，Imagen 。在 COCO 的 FID 分数（GAN 生成图像的分布与真实图像分布的「距离」，越小越好）和新测试基准 DrawBench 分数上都超过了 DALL.E。

但同时团队承认在训练数据集中加入了一些色情、种族主义和刻板印象等图像，在没有完善好保护措施前不提供给大众使用。

→ 官网

[Imagen: Text-to-Image Diffusion Models](https://imagen.research.google/)

---

7、Chineasy 是一款面向外语人士学习中文汉字的应用。整个应用有意思的点在于他们重新定义了象形文字：

![1669971083445.png](Scenes%20Weekly%20%2357.assets/1669971083445.png)

{上图：Chineasy 应用截图，来自 Screenlane}

→ 官网

[Chineasy | Award-Winning Chinese Learning Methodology](https://www.chineasy.com/)

---

8、YINGSTAR 工作室分享了上世纪一些古早教科书的插画部分。文末处那本数学书设计真的厉害。

→ 原文

[教科書類插圖](https://mp.weixin.qq.com/s/QUgRX5z_X-ViqZRfRpnWUQ)

---

9、最近 The Browser Company 对 Arc 浏览器开始新一轮测试，很遗憾没有体验到。但是可以看到这次测试版本是 0.99，基于 Chromium 101 版本，距离公测已不远。

在彭博社这篇新闻稿中可以看到其创始人 Josh Miller 的一些故事：

- Miller 建立 Arc 的初衷是，当前浏览器的布局以及拥挤的标签页，是浏览器行业停滞不前的证明；
    - 他认为所谓浏览器市场份额，只是代表其与服务的关联度。Chrome 集成了 Google 大量服务，并在 Android 默认安装。Safari 和 Edge 同理；
    - 像是 Chrome 的用户群体过于庞大，每个改动都要慎重考虑。理同微信；
    - 去年 iOS 15 Beta 版中大幅重设计了 Safari 界面布局，但意外不受大众欢迎，最后被迫妥协改为可选项。一位前 Safari 高级开发人员透露，此后团队变得更加保守，叹息；
- 作为一家产品还在测试的公司，[投资阵容](https://www.crunchbase.com/organization/the-browser-company/company_financials)太过豪华；

![1669971085274.jpeg](Scenes%20Weekly%20%2357.assets/1669971085274.jpeg)

{上图：Arc 的界面，功能都集中在可自定义的左侧边栏}

- Miller 眼中的 Arc 是一个在线操作系统，应用是每个 URL，所有的工作无需挤在一起的标签页去管理；
- 预定今年秋季公开发布；

→ 新闻

[Bloomberg - Are you a robot?](https://www.bloomberg.com/news/features/2022-05-27/google-chrome-and-apple-safari-challenged-by-browser-upstart)

---

10、Don't Wordle 是一个反 Wordle 游戏，你的目的不是在 6 步内猜出 Wordle 单词，而是尽量避免猜出最终答案。同时利用 Wordle 规则限制每一步输入的单词。

- 绿块字母必须在下一行的相同位置；
- 黄块字母必须在下一行的不同位置；
- 灰块字母不能出现在下一行；

这一切必须在六步内玩「躲避球」，如果 Valid Words Remaining 过少 ，可以撤回重新填写。例如我做的两次：

![1669971087102.png](Scenes%20Weekly%20%2357.assets/1669971087102.png)

{上图：左侧提前猜中 Wordle 游戏结束，右侧（故意）没猜中}

→ 比 Wordle 难多了

[Don't Wordle](https://dontwordle.com/)

---

11、Slashy 是一个自定义插件，可以设置各种 Notion 组合命令到一个「模板」中，还可以录像录音以及简单绘画。

→ 获取

[Slashy - Custom commands for Notion](https://slashy.app/)

---

12、内幕交易案的话题一般过于商业而不做讨论，但是 OpenSea 的这桩内幕交易是其前产品经理「利用关于哪些 NFT 将在 OpenSea 的主页上出现的机密信息，来获取个人经济利益」。聚合器平台的「喂养」（feed）在 web3 也适用于内幕交易，为 NFT 抹上一股浓重的灰色。

→ 新闻源

[https://www.cnbeta.com/articles/tech/1276293.htm](https://www.cnbeta.com/articles/tech/1276293.htm)

---

13、IINA 之前有过 HDR 分支 IINA+，最近终于在正式版中添加 HDR，利用上 mini-led 屏幕的出彩。Quick Time 虽然有出色的 HDR 表现，但是支持格式不如 IINA 多。而在 Infuse 中一些 HDR 测试视频显得有些过亮。IINA 是接近 QT 的，惊艳。

→ IINA 获取

[GitHub - iina/iina: The modern video player for macOS.](https://github.com/iina/iina)

---

14、Ty Mattson 主导过 Netflix Chilleez 玩具、FAO Schwarz 等知名品牌设计，他还有个星球大战海报的合作项目，Lucas 官方已授权。

![1669971089147.png](Scenes%20Weekly%20%2357.assets/1669971089147.png)

{上图：其中三张海报展示}

→ 观赏

[Star Wars x Ty Mattson - Ty Mattson](https://shop.tymattson.com/collections/star-wars-ty-mattson)

---

15、晚点的一篇报道，《中国互联网产品的无障碍改造：最难的不是技术》：

- 「技术问题之外，互联网产品的无障碍化程度依赖于公司决策者持续推进的决心、项目执行者平衡部门利益及解决冲突的智慧。」
- 「公司主动做无障碍化改造的动力一般有两个，商业回报或品牌回报。」
- 「在商业回报和品牌回报不足的时候，制度约束是最大推动力。」
- 「美团、支付宝等超级应用打开之后更像一个目录，各种功能层层叠叠，它们的排布更多取决于每个业务在庞大公司里的权力地位，而非用户体验。微信、今日头条、抖音等应用曾经简单，打开就是最主要功能，但也经年累月添加无数新功能，逐渐变成万能产品。把一款产品做成超级应用产品是中国移动互联网产品用流量带新品的必然结果。复杂的界面和繁重的功能对普通人已经不友好，更隔绝了视障人士。」

另外文中我还看到了这一句话：

> 使用电子密码锁时，杨欣才得用妻子拿硬纸板剪出的九宫格辅具，才能摸清密码锁上的数字在哪儿。

突然想到一种方法，即有没有可能做出把屏幕划分出不同区域的辅助手机壳，区域之间用实体的凸起触感分割，然后在实际设计 App 时，根据不同区域固定放置某些功能比如确认或返回，优化好的话甚至可以放弃 VoiceOver 式交互？然后不同的 app 类型可以适配不同的分割布局，这样一些简单的游戏也可以听过声音和触觉来更有效率地传递信息。

→ 原文

[中国互联网产品的无障碍改造：最难的不是技术](https://mp.weixin.qq.com/s/_M-voN7umvJUipC7Q2e-jw)

---

16、zk-Crush 这个网页小工具用途是，如何在不告诉你喜欢的人情况下，让对方知道你喜欢 TA。本质是[零知识证明](https://zh.wikipedia.org/wiki/%E9%9B%B6%E7%9F%A5%E8%AF%86%E8%AF%81%E6%98%8E)的小实验，实际操作是输入自己姓名和喜欢的人姓名，生成一段带有哈希值的网址，把网址发给别人，让对方输入自己姓名，一旦姓名相同便相当于哈希匹配成功，也就完成了表白（什么密码学神雕侠侣？）

→ 体验

[zk-Crush](https://www.zkcrush.xyz/)

---

17、 Sketch 采访了 GitHub 设计师 Gavin Nelson，询问了一些用 Sketch 画图标的心得。

→ 原文

[Made with Sketch: How Gavin Nelson puts the “icon” in “iconic”](https://www.sketch.com/blog/2022/05/27/gavin-nelson-icon-design/)

Figma 也发布了篇文章讲述开发可变字体功能的过程。原来他们请来了 Grilli Type 创始人 Thierry Blancpain 来做测试，本篇内容主要是对他的采访。

→ 原文

[Full-scale expression with Grilli Type](https://www.figma.com/blog/variable-fonts-a-conversation-with-grilli-type/)

---

18、Sliderland 和 [tixy.land](https://tixy.land/) 一样，使用 t（时间）、x（滑杆长度）、i（滑杆索引）构造数学函数式来制作圆滑的特效。比如你在灰框中输入以下公式就可以得到一个旋转的正方体。

```other
x>0.2-abs(sin(t*2))0.05&&x<0.8+abs(sin(t2))*0.05?(i%2?(min((x-sin(t%1.57)*0.3-0.5)*tan(-t%1.57)+cos(t%1.57)*0.3+0.5,(x-sin(t%1.57-1.57)*0.3-0.5)*tan(-t%1.57-1.57)+cos(t%1.57-1.57)*0.3+0.5)*0.4+0.5):(1-(min((-x-sin(t%1.57)*0.3+0.5)*tan(-t%1.57)+cos(t%1.57)*0.3+0.5,(-x-sin(t%1.57-1.57)*0.3+0.5)*tan(-t%1.57-1.57)+cos(t%1.57-1.57)*0.3+0.5)*0.4+0.5))):0.5
```

→ 试玩

[Sliderland](https://sliderland.blinry.org/)

---

19、也是上个月末，在 [Twitter 的视频](https://twitter.com/klevisl007/status/1530997381545738243)中可以看到某个人在卢浮宫的蒙娜丽莎扔蛋糕…… 好在有外面有防弹玻璃保护。视频中的男人在说（法语）：「有人在摧毁地球…… 所有的艺术家，想想地球吧。这就是我做出这种事的原因，多想想吧。」

1956 年有男子向蒙娜丽莎投掷石块，损坏了左边肘部，之后该画作一直置于玻璃后面。05 年还加固了外部，抵挡了一次 09 年被人投掷的空茶杯。

→ 新闻源

[Man arrested after Mona Lisa smeared with cake](https://www.theguardian.com/world/2022/may/30/mona-lisa-smeared-cake-suspected-climate-protester)

---

20、Depix 是一个 AI 驱动的在线图片编辑工具，可以轻松做到：

- 移除背景；
- 剪裁后的元素移动另一张图片上；
- 识别图片中的空间信息，在符合透视规则情况下添加元素；
- 一个特别的阴影系统；

→ 官网

[Image Creation: Online Image Editor Powered by Ai | Depix](https://depix.ai/)

---

21、一篇 Know Your Meme 总编 Don Caldwell 的采访文，原文已有完整的目录摘要：

- 什么构成 meme 以及内容何时超过 meme 阈值
- 揭示 meme 起源的艰苦过程
- Rickroll 和 wordcel 与 shape rotator 等 meme 的趋同演变
- 2012 年及以后的不同 meme 时代
- 在网络上闲逛的地方和社交媒体的成瘾性
- 技术的发展如何与 meme 的发展同步发生
- 接受 TikTok 是一个推动 meme 文化的大型互联网平台
- Web3 meme 以及你们中的一些人仍然不知道在单个猿上使用多个 slurp 果汁
- 最多产的 meme 一代以及为什么 Facebook 不仅仅是婴儿潮一代 meme
- 首席 meme 官和公司了解互联网 meme 文化

→ 原文

[帐号已迁移](https://mp.weixin.qq.com/s/fnkNql85icsSHEMdd_pNWg)

---

22、阿里健康大药房和方正联合发布了阿里健康体，包含中文、拼音和盲文。

→ 查看字体

[阿里健康体：字体无障碍，为所有人设计！](https://mp.weixin.qq.com/s/iJI_2foG2vwUCGY1AvkpDQ)

---

23、人们有多爱折腾纯文本呢？[第 36 期](./Scenes Weekly #36.md)介绍了非嵌入式标记语言 Aftertext 的语法，[第 48 期](./Scenes Weekly #48.md)介绍了纯文本版的 to-do 管理 [x]it! 。现在又有人想在纯文本里画线条和画圆。

Kartik Agaram 做了这么一个记事本，依赖于 LÖVE 这个 Lua 脚本框架。画了一条线后实际的文本格式为：

```lua
$ cat text

Hi there.

lines

{"p2":{"x":141,"y":85},"mode":"line","p1":{"x":34,"y":44}}

\

I am some text.

```

上面清除记录了线条坐标。如果要画圆的话，按住 O 不放开鼠标即可。

→ [更多介绍和下载](http://akkartik.name/lines.html)

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周更新了 0 个。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

---

# 劳逸

![1669971090933.png](Scenes%20Weekly%20%2357.assets/1669971090933.png)

{上图：Summer Game Fest}

这周继续过节。

本想周日晚上早点睡，结果还是边写本期通讯边把 Xbox & Bethesda 展会看了……

---

# 映像

现实拟像放映——

![1669971096460.png](Scenes%20Weekly%20%2357.assets/1669971096460.png)

{上图：路边黑色栏杆状建筑用橙色的线相互连接}

© Valentin Fougeray

---

# 温故

→ Scenes Weekly #8

[Scenes Weekly | No. 8](https://mp.weixin.qq.com/s/HUUCu2XZSP7CQLuh3f28sA)

- Big Mail 邮件客户端展示
- Boring Avatars 随机头像
- HarmonyOS 2.0 公布
- Spotify 颜色差异分析
- Twitter Blue 公布
- yourweek.app 极简 to-do 应用
- 用 Doom 当验证码

---

喜欢本文的话，欢迎分享、订阅。

第 56 期请[在此查看](./Scenes Weekly #56.md)。

本次封面使用了 Stardom 字体。

