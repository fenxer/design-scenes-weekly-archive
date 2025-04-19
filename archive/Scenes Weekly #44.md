# Scenes Weekly #44

2022-03-07

\> 设计视角下的世界——

第 43 期请[在此查看](./Scenes Weekly #43.md)。

本期出现：Framer Sites、Componentizer、Build in Public 、GIF、Capcom Logo、Screen Size、Telegie、User Interface Gallery、Product Hunt、Glitch Image Generator、Pro-tactile ASL

---

# 微博

1、我还没有拿到 Framer Sites 资格，所以只能看看 Brian Lovin 的第一印象——
优点：部署和发布很友好很便利；集成了组件系统；编辑器本身很精致很漂亮。
欠缺：无快捷键；布局系统与以往不太一样（对比 CSS Grid 或 Figma）；输出的代码尚有优化空间。

![5a519f71fee64d1f97e4bf25663d1d09.jpeg](Scenes%20Weekly%20%2344.assets/5a519f71fee64d1f97e4bf25663d1d09.jpeg)

{上图：Framer Sites 主界面}

总的来说持正面看法。

顺便一提，Framer 团队在 Lovin 直播中途就开始接受接受反馈了。

→ 原文

[Framer Sites first impressions](https://brianlovin.com/writing/framer-sites-first-impressions)

---

2、之前在每周通讯里（[第39期](./Scenes Weekly #39.md)）介绍过 Clover 的创始人 (at)attasi 做了一个反向组件化的插件 Componentizer。今天收到了 Beta 测试码用了一下，效果基本和官网首页的演示视频差不多。但没有视频里的 “Auto-Componentize” 功能，但是可以在 Advanced 里实现。

![5b2b1b317e5446c487739f134c776ed6.jpeg](Scenes%20Weekly%20%2344.assets/5b2b1b317e5446c487739f134c776ed6.jpeg)

{上图：Componentizer 高级选项}

如图所示，反向组件化的时候可以选择是否包含 Root Frame 和 Child Frame。而且插件支持检测 Overrides，减少多余的组件生层。毕竟做设计时，除了一些习惯性的元素会预组件化，在探索设计时 Componentizer 应该会提升效率，降低思考成本。

→ [官网](https://www.componentizer.design/)

---

# 摘录

> In popular culture we have “the bachelor pad,” and “the bachelor lifestyle,” but no such phrases for women. Women who live alone are objects of fear or pity, witches in the forest or Cathy comics. Even the current cultural popularity of female friendship still speaks to how unwilling we all are to accept women without a social framework; a woman who’s “alone” is a woman who’s having brunch with a bunch of other women. When a woman is truly alone, it is the result of a crisis—she is grieving, has lost something, is a problem to be fixed. The family, that fundamental social unit, dwells within the female body and emanates from it. Women are the anchors of social labor, the glue pulling the family, and then the community, together with small talk and good manners and social niceties. Living alone as a woman is not just a luxury but a refusal to bend into the shape of patriarchal assumption and expectation.

—— Helena Fitzgerald - [The Fierce Triumph of Loneliness](https://catapult.co/stories/the-fierce-triumph-of-loneliness)

---

# 杂事

1、自 Buffer 让公司包括财务在内的很多信息透明化，Joel Gascoigne 把 Build in Public 概念带到了人们眼前。以往公司内部的事情，整理并在社交媒体上放出来，公开一些奇特的想法或者一些功能的幕后故事，这样能尽早的从社区得到初步反馈；用户能感受到被聆听，继而增加忠诚度；自己可以一步步在社区建立话语权，从而吸引人才共事和新的投资机会。

Failory 的这篇文章介绍了 Build in Public 几个点，包括分享内容的类型、分享渠道，也提到了有些公司停止 Open 的原因。顺便一提在独立游戏开发领域，Build in Public 已是常态。

→ 原文

[Building in Public: 20 Examples & a How-To Guide](https://www.failory.com/blog/building-in-public)

---

2、最快的 GIF 是什么样的？我们都知道动图之间的帧延迟越低，GIF 就会动的越快。那么延迟为0ms呢？ 这篇文章探索了浏览器环境下渲染 GIF 的延迟处理。

![AnimatedImage.gif](Scenes%20Weekly%20%2344.assets/AnimatedImage.gif)

{上图：调节不同的延迟时，不同的 GIF 速率}

如上图可以看到 0ms 延迟时，速率其实好 100ms  相同。这归根在于浏览器「不支持」 0ms 延迟的 GIF。绘制帧太快会占用额外的性能，而且会被恼人的动图广告滥用。不同的浏览器限制条件不同，比如 Chrome 一般情况下对任何小于 10ms 的帧延迟都会被标准化为 100ms。所以 20ms 的动图反而动得最快。

→ 查看原作者的更多想法

[The Fastest GIF Does Not Exist](https://www.biphelps.com/blog/The-Fastest-GIF-Does-Not-Exist)

---

3、去年滨口龙介凭《ドライブ・マイ・カー》（驾驶我的车）夺得数枚影展奖项，并在奥斯卡非外语片中得到 4 项提名。这篇文章摘取翻译了奉俊昊和滨口龙介的对谈，从车内拍摄、对话表现手法到对演员的指导进行了交流。

→ 全文

[【奉俊昊 ╳ 濱口竜介】上篇：拍一場對話，有時比動作戲還難 ｜ BIOS monthly](https://www.biosmonthly.com/article/11004)

---

4、上上周 Capcom 上线了一个倒计时网站，大家都以为生化危机系列某部重置消息即将到来，但结果是街霸6……倒也还行，看到了上了年纪的隆。但是 PV 结尾的标识却让人感到迷惑：

![SF.png](Scenes%20Weekly%20%2344.assets/SF.png)

{上图：左边为街霸的六代标识（暂），右边为 Adobe Stock 付费素材}

以往的街霸 logo 都是带有强烈的书法元素，这次不伦不类的图形让人怀疑这可能只是个占位图，如果真是正式标识的话，那就贻笑大方了。

---

5、Screen Size 迭代到了2.0 版本。在原本方便地查看屏幕分辨率的同时，增加了大量其他屏幕信息和大量改动。

![Screen Size.jpeg](Scenes%20Weekly%20%2344.assets/Screen%20Size.jpeg)

{上图：Screen Size 2 各平台截图}

→ 查看

[Screen Sizes](https://www.screensizes.app/)

---

6、几年前 Capture 这个应用让我感受到了前置的深感摄像头魅力，它能够通过简单的拍摄物体直接转化为 3D 模型。3d Scanner App 也是类似原理，但支持的机型有限。最近 Hanseul Jun 又做了一个叫 telegie 的小应用，可以录制 RGBD 视频然后上传到网页查看。同时支持 AR/VR 浏览。

→ 作者在HN发的帖

[Show HN: I made an iOS app recording RGBD videos and a web app playing them | Hacker News](https://news.ycombinator.com/item?id=30437257)

---

7、那个之前做过 ui.wtf 和 Ultra 的等实验性项目的 Rauno Freiberg，又上线了 User Interface Gallery。

![截屏2022-02-25 00.29.57.png](Scenes%20Weekly%20%2344.assets/%E6%88%AA%E5%B1%8F2022-02-25%2000.29.57.png)

{上图：按钮历史作为展示其中一项}

→ 有想法

[User Interface Gallery](https://ui.gallery/)

---

8、Ian Wootten 通过 Product Hunt 老接口抓取了9万多个产品的信息，然后检测其链接（大多是官网）的 HTTP 状态码来验证产品是否还活着。

![response.png](Scenes%20Weekly%20%2344.assets/response.png)

{上图：各产品链接状态码一览}

如上图，2开头和3开头（重定向相关）的状态码可以代表产品依然存活，剩下22.4%的产品都返回了错误状态码（4开头是请求错误，5开头是服务器错误）。这些产品中，含有 no-code 标签出错百分比最少，意味着大多数 no-code 产品都会比较持久。而带有众筹标签的产品是链接错误最多的，这也跟众筹本身的性质有关。

→ 查看更多信息

[Are Product Hunt's featured products still online today?](https://www.scrapingbee.com/blog/producthunt-cemetery/)

---

9、Glitch image generator 是一个自动生成故障图像的网页工具。原理看起来是生成不规则条状矩形错位蒙版，通过不同的叠加模式来生成图像。

![截屏2022-02-26 13.56.27.png](Scenes%20Weekly%20%2344.assets/%E6%88%AA%E5%B1%8F2022-02-26%2013.56.27.png)

{上图：示例图片}

→ 地址

[Glitch Image Generator](https://glitchyimage.com/)

---

10、一个2016年的视频，内容是 Pro-tactile ASL 的介绍。这个语言由聋盲人社区发展，证明了语言除听觉和视觉外，还可以用触觉传递。

→ Youtube

[Pro-tactile ASL: A new language for the DeafBlind](https://www.youtube.com/watch?v=9GrK3P15TYU)

→ 腾讯视频（已翻译）

[Pro-tactile ASL聋盲人的另一种交流方式！_腾讯视频](https://v.qq.com/x/page/y06536hdtfc.html)

---

# 劳逸

![30e5d20cdae84ca58c94cb0f92d8b1d8.jpeg](Scenes%20Weekly%20%2344.assets/30e5d20cdae84ca58c94cb0f92d8b1d8.jpeg)

{上图：Card Shark 商店页截图}

「以出千的方式一路走进 18 世纪的法兰西上流社会。精通各种骗术，熟练运用标记卡牌、假洗牌、切换牌堆、假发牌等技巧！凭借你赚来的不义之财，进入高风险赌桌的秘密世界。」

Card Shark 这游戏是真的想教会你出千，里面包含了近30个千术，用精致的动画和神奇的交互向你演示，一次学不会还可以往复练习……游戏目前只有 Demo 版（Steam Demo 节）。不说了，该继续艾尔登法环……

→ 游戏获取

[Steam 上的 Card Shark](https://store.steampowered.com/app/1371720/Card_Shark/)

---

# 映像

现实拟像放映——

![f543b135262347a5af8cb02c05c7f728.png](Scenes%20Weekly%20%2344.assets/f543b135262347a5af8cb02c05c7f728.png)

{上图：带胡须的蒙娜丽莎}

《391》第12期刊登的杜尚的L.H.O.O.Q。图源为 Duchamp Research Portal 组织中费城艺术博物馆提供。该网站公示了很多杜尚的资料。

→ 详见

[https://www.duchamparchives.org/pma/object/254544/](https://www.duchamparchives.org/pma/object/254544/)

---

喜欢本文的话，欢迎分享、订阅。

第 43 期请[在此查看](./Scenes Weekly #43.md)。

本次封面使用了 DeepMind Serif Display 字体，图形灵感来自 JOJO。