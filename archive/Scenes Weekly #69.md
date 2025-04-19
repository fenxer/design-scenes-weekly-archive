# Scenes Weekly #69

2022-09-13

\> 设计视角下的世界——

第 68 期请[在此查看](./Scenes Weekly #68.md)。

本期出现：

- 灵动岛设计小前瞻
- Zenly 怀念小前瞻
- 重读 HIG 小前瞻（十）
- 最短的域名小前瞻
- YouTube 变速功能小前瞻
- Stable Diffusion 三则小前瞻
- 其他小前瞻：meme 产出平台统计、Mobbin 大更新、探索iOS导航建议、Craft 更新、PowerToys 更新

如有格式异常建议点击最上方「在浏览器中访问」。

---

节日快乐。

由于没怎么出家门所以有了一些时间来随便写写。

欢迎上周的新订阅者，感谢所有订阅者的支持。

---

# 月圆

1、灵动岛（Dynamic Island）让大众目光重回系统界面设计，优秀的动效取悦并缓解了很多人对不完整屏幕的排斥。另一边无论是否是「刘海」的拥护者都涌入了「守旧派」，这里的人都对一块如满月般完整的圆角屏幕有着很深的执念，并批评 Apple 的创意匮乏与本末倒置。

我对灵动岛完整的设计工作量持正面看法，它兼顾了 Apple 设计的秩序与自由，进一步强调了移动系统的屏幕「状态展示」——这在桌面端操作系统很常见。但如果究其本质是从硬件出发，我又很失望。首先「刘海」操作区早在五年前第一个全面屏 iPhone X 发布时，就被具有搞怪天赋的设计师们畅想了这块空缺的未来，比如[这个](https://dribbble.com/shots/3965749-Pull-The-Notch)、[这个](https://dribbble.com/shots/4247369-Loading-notch)和[这个](https://dribbble.com/shots/3824298-Pull-to-refresh-iPhone-X-edition)，还有[这个](https://dribbble.com/shots/3817535-iPhone-X-Mail-App-Concept)。此时的「刘海」是一块不规则的区域，并且与外边框相连，决定了它是外边框的一部分——边框是静止的。

![充电时结构.png](Scenes%20Weekly%20%2369.assets/%E5%85%85%E7%94%B5%E6%97%B6%E7%BB%93%E6%9E%84.png)

{上图：充电时灵动岛所变换的设计结构，蓝红两边放置信息，中间为前置摄像部分}

而「药丸屏」切断了外边框的联系，给予了该区域与内部建立联系的机会。于是「不甚创新」的灵动岛抓住了这个机会登上了交互舞台。

![Frame 12.png](Scenes%20Weekly%20%2369.assets/Frame%2012.png)

{上图：以三种颜色标记展开后的灵动岛与四周边距，红色上边距约等于绿色半径边距，并小于黄色边距}

不过既然是以黑色为背景，不知道能不能向小组件一样成就一批开发者。而使用黑色联动硬件，在 [Apple Watch](https://designscenes.zhubai.love/posts/2160656211648229376#:~:text=%E7%B3%BB%E7%BB%9F%E8%83%8C%E6%99%AF%E6%98%AF-,%E7%BA%AF%E9%BB%91%E8%89%B2,-%EF%BC%88%23000%EF%BC%89%EF%BC%8C%E6%84%8F%E5%9B%BE%E6%98%AF) 上便有着不错的扩屏效果。9To5Mac [这篇文章](https://9to5mac.com/2022/09/08/iphone-14-pro-how-dynamic-island-works/)使用 Xcode 的模拟器探索了更多灵动岛的机制。

更多对灵动岛的探索还是等到实机到手（排队到十月份了），因为我很好奇黑色覆盖的有多沉浸，以及具体的点按区域。在结束思考前我看了一眼 RTL 版灵动岛布局，原来字段同样没有太长。

![DI-RTL.png](Scenes%20Weekly%20%2369.assets/DI-RTL.png)

{上图：阿拉伯语下的灵动岛界面}

---

2、8 月 31 日，Snap [宣布](https://newsroom.snap.com/restructuring-and-refocusing-our-business)重组业务并将逐步关闭 Zenly 在内的一些应用，市面上又少了一个很酷的产品。Jacob 梳理了 Zenly 如何解决地图社交应用的几个挑战：

- Zenly 团队构建了 ZenEngine，以实兼容省电和精确定位，让用户持续分享位置坐标，成为了产品体验的基石；
- Zenly 将自己定位为线下的位置共享，看重与现实世界的联系而不是单纯的 LBS 工具，用来回应外界对隐私的质疑；
- 应用本身也加强了对隐私的控制，有一键消失的 ghost mode 和定向分享；
- 出色的游戏化设计容易让更多人乐于分享；
- Zenly 虽然不能做到像 Google 地图一样的数据准确性，但是做好了这些数据大厂都没做到的社交融合；

![1500x500.jpeg](Scenes%20Weekly%20%2369.assets/1500x500.jpeg)

{上图：Zenly Your World}

→ [原文](https://www.makingproductsense.com/p/location-sharing-in-a-skeptical-world)

---

3、Know Your Meme 截取记录了 2010 - 2022 年间每年 700-1400 个 meme 发源地，来查看每年哪个平台/社区产出的 meme 最多，也是十几年来社交平台的兴衰见证。

→ [原文](https://knowyourmeme.com/editorials/insights/where-do-memes-come-from-the-top-platforms-from-2010-2022)

---

4、专注于移动应用界面分享的 Mobbin 更新了他们的品牌，并增加了流程展示（Flows）。分享这些界面的网站不算少，但是更新稳定、内容充实的大概只有 Mobbin 在坚持。

![mobbin.png](Scenes%20Weekly%20%2369.assets/mobbin.png)

 {上图：Mobbin 的新标识}

→ [说明](https://twitter.com/MobbinDesign/status/1567082719657742336)

---

5、腾讯微信设计中心这篇文章结合了 WWDC22 [Explore navigation design for iOS](https://developer.apple.com/videos/play/wwdc2022/10001/) 视频和国内应用生态，来讨论应用首页和常驻导航栏「水土服不服」。

We-Design 之前也是潜心下来写文章，不只做 showcase，挺好的。

→ [原文](https://mp.weixin.qq.com/s/qN9qS8lfmhuzweceBxPYQA)

---

# 重读HIG（十）

本节是重读 Human Interface Guidelines 系列连载第十期，目的为温故知新和跟进新内容。 为避免篇幅过长，不会一次发布太多，之前内容已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上。

### 输入数据（Entering data）

首先对输入数据的一个预期是，无论人们使用哪种交互，输入数据都是枯燥无聊的。尽可能减少需要输入的工作量，是优化体验的一个重要工作。

减少工作量可以从系统获取信息，或者使用控件选择输入方面入手，但是涉及隐私的密码字段就不必预填充，填充前务必使用机器密码或者生物特征识别等验证机制。

最好是动态地验证字段是否合规，及时修改。

macOS 上可善用 [tooltips](https://developer.apple.com/design/human-interface-guidelines/patterns/offering-help/#macos) 帮助用户理解表单。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/entering-data)

### 反馈（Feedback）

反馈可以传达过去、现在和未来的信息，向用户展示交互结果、当前交互状态和交互预测信息。

HIG 原文的第一点很重要，反馈的前提是保证用户能收到反馈，包括那些使用辅助功能的障碍用户。

🤔 其他点暂时觉得没必要再拿出来讲了，详见原文。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/feedback)

### 全屏（Going full screen）

全屏模式可以给当前应用带来沉浸的感受，但并不是每个应用都需要全屏，比如 macOS 上的计算器。

全屏时，（macOS）边缘或（iPadOS）底部触发 Dock 栏可以让用户快速切换应用。但沉浸的游戏应用除外，比如 iOS 和 iPad 游戏中只有多次触发 Home Indicator 小横条才会触发后续交互。~~至于 macOS 我已经忘记上次拿 Mac 玩游戏是什么时候……~~

在 [Layout](https://developer.apple.com/design/human-interface-guidelines/foundations/layout) 一节谈到了各个设备的安全区问题，但是唯独 macOS 设备被一笔带过。对于带刘海（notch）的 MacBook 型号，全屏默认低于刘海区域。同时 Apple 提供 [auxiliaryTopLeftArea](https://developer.apple.com/documentation/appkit/nsscreen/3882915-auxiliarytopleftarea)和[assistantTopRightArea](https://developer.apple.com/documentation/appkit/nsscreen/3882916-auxiliarytoprightarea) 来定制刘海两侧空间的显示内容。不过至今没遇到什么具体案例。

![macOS full.png](Scenes%20Weekly%20%2369.assets/macOS%20full.png)

{上图：带「刘海」的 MacBook 全屏时的几个区域}

始终允许 macOS 用户能触发 Mission Control，不要占用其快捷键和手势。

一些应用离开全屏时，可以默认帮助用户暂停当前流程。比如游戏或者视频。视频的话还可以选择继续背景播放或自动变为画中画，游戏也可以有不暂停但降低帧率等优化选项。当然还有一些「明显的」应用就不必了，比如下载器、音乐播放等。具体场景具体考虑，原文并没有说清楚这一点。

 macOS 上进入全屏后，除非用户主动了解并退出全屏模式，否则尽量在全屏模式下完成打开、导入和保护文件等类似交互，而不中断全屏。在 iOS 和 iPadOS 上的全屏则是一个很约束的场景，iOS 没有多窗口，iPadOS 上没有多桌面，多任务处理依然比较薄弱。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/going-full-screen)

---

# 摘录

这周看过的一些——

> Things get more refined as you make mistakes and do them, so I’ve had a chance to make a lot of mistakes.

> Your aesthetics get better as you make mistakes.

> But the real big thing is that—the way I’ve always felt—is that if you’re going to make something, it doesn’t take any more energy and rarely does it take more money, to make it really great.

> All it takes is a little more time—not that much more—and a willingness to do so: a willingness to persevere until it’s really great.

——  Steve Jobs [Interview with Michael Moritz](https://stevejobsarchive.com/interview-with-michael-moritz) - Steve Jobs Archive

# 花好

6、笔记应用 Craft 发布了 Windows 客户端，很遗憾只是 ”Windows-specific app” 而不是 native app，使用了 Electron 封装了是同一期发布的 Web App 1.0。使用时文章区域还会有原生的滚动条（即便设置中已关闭默认展示滚动条），文本对缩放的支持也不太好，改进之处还有很多。

→ [更新原文](https://www.craft.do/s/sh9bQ3y27tRnIS)

---

7、Windows 开源之光 PowerToys 新加入了 OCR 功能，基于 [Text-Grab](https://github.com/TheJoeFin/Text-Grab)， 识别英文很方便，识别中文的话每个字之间会有空格，日文假名基本无法识别，有点像 macOS 早期的 Live Text……

![屏幕截图 2022-09-12 174241.png](Scenes%20Weekly%20%2369.assets/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202022-09-12%20174241.png)

{上图：PowerToys 0.62 版本已有很多小工具}

→ [获取](https://github.com/microsoft/PowerToys)

---

8、世界上最短的域名是什么？Google 的 `g.co` 和 Facebook 的 `m.me` 都不是最短的，James Williams 找到了一些被解析的顶级域名（TLD）——有些域名注册商是不会放过 TLD  A记录的。

 Williams 在 [iana](https://www.iana.org/) 域名库中寻找，筛选后找到了几个返回 DNS 记录的 TLD。

```javascript
AI	209.59.119.34
CM	195.24.205.60
PN	139.162.17.173
TK	217.119.57.22
UZ	91.212.89.8
WS	64.70.19.33
XN--L1ACC	218.100.84.27
```

这里面 [http://ai](http://ai) 有一套完整的页面，用来宣传安圭拉的离岸服务（.ai 是安圭拉注册的 ccTLD）。[http://pn](http://pn) 只有 “It works!” 和一小段文字。

理论上，ICANN 也可以将根区解析到 A 记录，这样 `http://.`  和 `http://`  就是最短域名了。不过一是 ICANN 本身不鼓励这样添加 A 记录，二是浏览器大概率也会认为这是空链接。

→ [原文更详细](https://jameswillia.ms/posts/shortest-urls.html)

---

9、Youtube 的官方博客告诉大家，人们使用变速功能一般是加速 1.5 倍，其次是 2 倍然后是 1.25 倍。虽然正常速度看视频时主流，但是变速这个功能已经成为视频播放不可或缺的一个功能。

- 在智能电视或者游戏主机上，正常播放速度人数最多，其次是 1.25 倍速度，在网页上则是 2 倍速播放；
- iOS 和 Android 移动端最常使用 1.5 倍速播放；
- 晚上 11 点是使用变速功能的高峰期；
- 随着早上到晚上，人们的播放速度越来越快；
- 有些用户还想加入 3 倍甚至 4 倍速度播放；

→ [原文](https://blog.youtube/inside-youtube/youtube-watch-video-playback-speeds-trends/)

---

10、Stable Diffusion 三则——

10.1、社区用极大的热情回应了 Stable Diffusion 的慷慨开源，以至于几乎每周有新事物吸引眼球。Lexica 是一个搜索 AI 生成图片的网站，可以根据图片本身关联性或描述文本（prompts）搜索图片。Lexica 会根据 prompt 的特征做分词搜索，并附有每张图片的 Seed、Guidance scale 和分辨率。

![截屏2022-09-12 22.39.22.png](Scenes%20Weekly%20%2369.assets/%E6%88%AA%E5%B1%8F2022-09-12%2022.39.22.png)

{上图：Lexica 搜索结果页面}

→ [试试手气](https://lexica.art/)

---

10.2、Andreas Jansson 在 Replicate 运行了一个动画版 Stable Diffusion。给出起始和结束两段描述文本，就可以生成动画，如下图。

![AnimatedImage.gif](Scenes%20Weekly%20%2369.assets/AnimatedImage.gif)

{上图：默认展示案例}

动画还用到了 [Google FILM](https://replicate.com/google-research/frame-interpolation) 插值。

→ [体验](https://replicate.com/andreasjansson/stable-diffusion-animation)

---

10.3、上次介绍过 Stable Diffusion 的 WEB GUI 安装，现在直接有了 Diffusion Bee 这种一键安装打包，该来的总会来。

Diffusion Bee 完全在本地运行，需求至少 16GB 内存和 M1/M2 芯片的 Mac 设备。但目前还不支持 seed 和 image to image 功能。

自己测试了下，确实很吃性能，需要尽可能关闭其他应用使用。

![t2i@2x.png](Scenes%20Weekly%20%2369.assets/t2i@2x.png)

{上图：运行文字转图像时机器内存占用}

→ [体验](https://github.com/divamgupta/diffusionbee-stable-diffusion-ui)

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

~~现在玩游戏也要放假。~~

---

# 映像

现实拟像放映——

![leaf.png](Scenes%20Weekly%20%2369.assets/leaf.png)

{上图：使用M3 螺丝和螺杆，串上树叶，俯视看就像人脑的CT图}

HAPPENS IN BETWEEN

[© K.Chen](https://k-chen.nl/)

---

# 温故

→ [Scenes Weekly #20](https://mp.weixin.qq.com/s/68ZgH0XI4ClIpnoTDyJJ8g)

- SigmaOS 浏览器劝退体验
- 取消订阅 Adobe CC 计划的糟糕流程
- Figma Widget 功能
- 机器翻译的过去、现在和未来
- FlickType 被迫下架
- Paint Transformer 笔刷生成绘画过程
- 专辑封面 showcase 网站 suupcover
- 公益项目 Flowers For Sick People
- 为什么超链接默认是蓝色的
- 字体筛选网站 Font Brief 
- 网页搜索语言模型 Wanderer2
- 验证 HN 是否可以衡量未来技术趋势
- 现代 Dos 游戏库 Dos Haven
- 可变字体实验：西文 A 到平假名 あ
- 磁带和 VHS 录像带的包装设计

---



喜欢本文的话，欢迎分享、订阅。

第 68 期请[在此查看](./Scenes Weekly #68.md)。

本次封面使用了 Partita 字体，灵感来自动画中的原画定位纸。