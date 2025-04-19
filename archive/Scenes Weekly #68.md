# Scenes Weekly #68

2022-09-05

\> 设计视角下的世界——

第 67 期请[在此查看](./Scenes Weekly #67.md)。

本期出现：

- 平均值定义下的用户标签
- Twitter 新信息摘要卡片
- 简单使用网页检测 iOS 是否开启锁定模式
- 重读HIG（九）
- DreamStudio 更新简介
- mimic 再次激起伦理讨论
- 深挖 Microsoft 与 Figma 关系
- 其他：汉仪字体上市、政商备忘录收集、 Twitter 测试编辑功能、Meta Widely Viewed Content Report、营销广告小贴士、Accessibility Not-Checklist、蒙纳收购 Berthold 字库、Nvidia 市场趋势分布、Sony 探头手游

如有格式异常建议点击最上方「在浏览器中访问」。

---

上一期的唠科隆那里引用了大量 bilibili 链接，推送后才反应过来可能会触发 spam 警报进入邮件垃圾箱，之后会注意下同一域名链接数量和密度。同时因为竹白的推送出了些问题导致一些人晚收到了邮件，抱歉。

为了防止之后邮件误进入垃圾箱，你可以对邮件对话做上标记（比如 Gmail 中标记重要对话），添加邮件联系人或者制定过滤规则等等🙏🏻。

最后，欢迎上周的新订阅者。感谢所有订阅者的支持。

---

# 小事

1、来自上周的 [Design Lobster](https://designlobster.substack.com/p/-5-more-ideas-about-design#%C2%A7-be-skeptical-of-averages)：

> 上个世纪 50 年代初，飞行员事故多发。美国空军认为原因是 20 年代后飞行员平均体型发生了变化，邀请了人类学家 Lt Gilbert Daniels 来进行人体测量学研究并修正相关数值。Daniels 测量了 4000 多名飞行员，指标包括腰围到眼距等 10 个维度。超出军方预期的是，没有飞行员在测量出的所有指标的平均值内。换言之，以平均值指标打造出的驾驶舱不适用于所有人，事故的原因便来自这个错误的前提。

> 解决方案是使驾驶舱各个装置可调节，以适配每个人的体型。

→ [原视频](https://www.youtube.com/watch?v=PNxCGNFyDE4)

> 📬 回溯：在[第 63 期](https://designscenes.zhubai.love/posts/2165749375996317696#:~:text=%E6%9C%AC%E9%80%9A%E8%AE%AF%E4%B8%AD%EF%BC%8C%E3%80%8C-,%E7%94%A8%E6%88%B7,-%E3%80%8D%E4%B8%80%E8%AF%8D%E5%85%B6%E5%AE%9E%E6%98%AF)重读 HIG 的包容性（Inclusion）一栏中提到：

> 个人看法，在中文语境包括在本通讯中，「用户」一词其实是被标签化的结果。主语是「人们」的时候，是在叙述大环境背景下的一般人。而「用户」则指代被抽象化的人群，这个人群以第三方视角描述时，带有特定的含义。

很多产品想要增长，想要吸纳更多的用户，为商业化的桥梁做设计，基于业务模式的考量和前人经验，所诞生的产品模块越来越雷同，服务于用户中的多数派。这里面的用户是被量化为平均值的，即便是「设置」里的选项也并未基于个体而是产品本身的扩展。

Jacob Jolibois 的一篇文章提到了那些特立独行的产品应用，像是：

- 每月支出数十美元给邮件分类的 Hey；
- 每天不定时间突发拍照上传的 BeReal；
- 丢掉书签重新认识网页标签管理的 Arc；
- ……

这些产品 GTM 是去寻找具有相同愿景的人成为他们的用户，显然它们不适合每个人，也可能会做出错误的决策，甚至本身有些难用，但这些产品没有平均化用户个体，在「平均值范围」外构建设计正是它们意义所在。

→ [原文](https://www.makingproductsense.com/p/opinionated-software)

> 📬 回溯：[Camera Obscura: Beyond the lens of user-centered design](https://alexis.medium.com/camera-obscura-beyond-the-lens-of-user-centered-design-631bb4f37594)

> Alexis Lloyd 的这篇文章更像是从政治哲学角度去切入 UCD（以用户为中心）的盲区。UCD 作为体验设计的中心已有多年，近年来也开始兴起中心区域之外的讨论，例如本文提出的三种观点：传统 UCD 所谓的 ”User” 范围已变得狭隘；对于设计的优化背后矛盾的转移；对于交互路径定义单一等问题，无不让 UCD 落入功利主义的陷阱。

> Lloyd 提出以 actor 作为 user 的替代，以参与者的名义包含了使用者（原用户）及其影响到的人。在设计创造的这个“世界”里，世界系统的规则决定了各参与者的利益，利益的分配又会反过来让规则产生波动。我们应在保持规则开放的同时，去探索各利益线索背后的源头，比如原文提到的三点：

- > What’s the worst thing a user can do with this system?
- > Who are my most vulnerable participants?
- > Why are the bad actors incentivized to act this way? What do they gain?

> 多去设定结果、落实到 system map、回归道德主义，都可以在这条新道路上走的更远。



> 💡 拓展：[为何强调“易用性”的智能手机交互逻辑对老年人来说存在障碍？](https://mp.weixin.qq.com/s/Ax4bhnvXf1K7x_JeaRqtAQ)

> 人固有认知的误区就在于觉得「人」都是一样的，讨论书的时候还分文学，哲学，历史或科技，回到这类问题上，人就只是「人」了。平时还会说人的个性是不同的，人是有族群的，人是有聪明的和愚笨的，善恶的或奸诚的，但只要聊到人类行为的时候，人突然就被统一了。这是个很有意思的问题。

---

2、Twitter 开始测试更丰富的信息摘要卡片（Tweet Tiles），主要是针对新闻媒体行业。比普通的摘要面积更大，标题和媒体品牌可自定义显示样式，以及明显的 CTA 按钮。

![截屏2022-09-02 14.27.26.png](Scenes%20Weekly%20%2368.assets/%E6%88%AA%E5%B1%8F2022-09-02%2014.27.26.png)

{上图：Twitter 公布的视频中，新摘要卡片样式预览}

目前仅开放给三家媒体账号使用，《纽约时报》、《华尔街日报》和《卫报》。新样式测试的是一半人能看到新样式作为实验组，而另一半人看不到，典型的 A/B Test，测试的结果很大可能是正面的（新样式带来的好奇心）。

媒体一侧则是在网页 <head> 中引入新的内容协议 `name=“twitter:XXXX”`，如下图。

![截屏2022-09-02 12.48.05.png](Scenes%20Weekly%20%2368.assets/%E6%88%AA%E5%B1%8F2022-09-02%2012.48.05.png)

{上图：《华尔街日报》新闻页面，代码头部添加的 Twitter 专用内容协议}

可以看到实际的协议种类和 [The Open Graph protocol](https://ogp.me/) 一样丰富……《卫报》那边则是只引用了 `twitter:app:XXXX` 这一格式。而在我的 iOS 客户端（9.26 版本）并没有看到新样式。

目前还没有相关文档可供阅读，也尚不清楚未来是否会开放给更多类型媒体。

→  [公布推文](https://twitter.com/ashevat/status/1562862418514288640)

> 📬 回顾：[A/B Test Hypotheses are Broken, Here’s What We’re Using Instead](https://growthrock.co/a-b-test-hypotheses/)

> 电商测试服务网站 GROWTH ROCK 发布了一篇文章探讨了 A/B Test 背后的种种虚假的表象——因涉及内外部的利益而导致的测试时间不足（样本量不足）轻易定下结论；同样因利益原因导致的测试结果单一性，只是为了数据好看而产生偏见……

> GROWTH ROCK 建议不是以真正去测试的心态去进行 A/B Test ，而是在保持测试初心的同时探索整个流程的各项指标去质疑和解疑。

---

3、Apple 在七月份推出了锁定模式（Lockdown Mode），以在极端情况下应对 Pegasus 等间谍软件。

![Lock.png](Scenes%20Weekly%20%2368.assets/Lock.png)

{上图：iOS 16 测试版已推出的锁定模式}

在该模式的众多限制中，就包括了无法加载网页的自定义字体。所以反过来检测浏览器是否支持自定义字体便可以了解到网站访问者是否开启了锁定模式——你知道的，普通人一般不会开启锁定模式。

专注于隐私空间的 Cryptee 推出了一个验证网页 demo，公司 CEO John Ozbay 说这个网页开发五分钟就能搞定，核心检测 JS 为：

```javascript
 /**
  * Checks to see if user has iOS Lockdown Mode enabled.
  */

  function detectIOSLockdownMode() {
  		if ((isios || isipados || isSafari) && iOSversion()[0] >= 16) {
       	breadcrumb('[LOCKDOWN MODE] Testing...');
         	fontSpy('remixicon', {
           	glyphs: '\uf2d1\uf2d2\uf2d3\uf2d4\uf2d5\uf2d6\uf2d7\uf2d8\uf2d9',
              success: function () {
              	// fonts loaded
                 userIsNotInLockdownMode(); // not in ios / safari / lockdown mode
				},
              failure: function () {
              	detectedIOSLockdownMode(); // in ios / safari / lockdown mode.
              }
           });
		} else {
       	userIsNotInLockdownMode(); // not in ios / safari / lockdown mode
       }
}
```

这不是锁定模式有疏漏，而是因为其严谨性反而在冲浪时显得更突出。而且这对大多时候的大多数人来说都是一个隐形功能。

→ [新闻原文](https://9to5mac.com/2022/08/26/iphone-lockdown-mode-2/)

（未完待续）

---

# 重读HIG（九）

本节是重读 Human Interface Guidelines 系列连载第九期，目的为温故知新和跟进新内容。 为避免篇幅过长，不会一次发布太多，之前内容已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上。

## 拖放（Drag and drop）

HIG 描述拖放的术语：

- 选择起始内容的位置，称为 source；
- 拖放到另外的位置，称为 destination；
- 两者可能在，也可能不在同一容器中，甚至是不同的应用程序；
- 这两个单词会出现在一系列声明方法中，包括不使用拖放完成拖放操作的辅助功能[1]；

[1]: [accessibilityDragSourceDescriptors](https://developer.apple.com/documentation/objectivec/nsobject/2891001-accessibilitydragsourcedescripto) 和 [accessibilityDropPointDescriptors](https://developer.apple.com/documentation/objectivec/nsobject/2891048-accessibilitydroppointdescriptor)

HIG 建议支持批量拖放和撤回拖放操作。

- 也考虑支持 spring loading。这个抽象的词组指的是在拖放过程中，移到某些控件上仍然可以激活。最常见的是拖放文件操作，拖着文件移到文件夹或者返回/前进控件上，一定延迟后便可访问或激活，[详见演示](https://developer.apple.com/videos/play/wwdc2020/10206/?time=1032)。

拖放是一个有着「起因经过结果」的动态过程，需要为用户提供清晰的反馈：

-  一旦用户长按拖动内容超过 3pt，应立即显示不同的图像来表示进入拖放状态；
- 修改拖放图像帮助用户预测目标位置（destination）；
- 告诉用户能否将内容拖放到当前位置；
- 拖放无效时，也提供反馈，比如移回到原位置（source）或者缩放后淡出；

其他建议：

- 目标位置的内容可在拖放时触发滚动（比如移到容器边缘）；
- 对于拖放内容，尽量保留原内容格式（包括文本样式）。或者对于特定输入区域，仅摘取可用信息。不兼容的话再考虑生成图像；
- 设备连接实体键盘时，按住 Option 即代表在当前容器复制内容（意思是不要用于其他交互）；
- 提供一个拖放内容的时间和状态进度条；
- 拖放后，一般建议保持选中状态；

---

说实话，拖放这节写的并不好，HIG 没有生动易懂地展示拖放交互各个细节。

而且很多点 Apple 自己的系统和其他常有应用程序也没有落实到位。

一个对拖放交互象比较深的印象是，从 iOS 相册长按图像主体，触发「抠图」，此时主体可以自由拖动，移到任何组件上均无反馈（没有支持 spring loading）。只能使用另一只手指操作，比如进入多任务界面，选择微信，依然不支持 spring loading。直到点进聊天界面，也没有出现不可拖放的提示。如果拖到备忘录中，则会在拖动图像上显示加号。

![Drag Drop.png](Scenes%20Weekly%20%2368.assets/Drag%20Drop.png)

{上图：一些没有反馈的拖放操作，感谢「小锅」的友情出演}

同理上图最右，拖拽通讯录中的联系人也没有任何显示反馈，拖放无效。

Drag and drop 这一节开始便说道：

> **As much as possible, support drag and drop throughout your app.** Most people are familiar with drag and drop and they often try it everywhere. When you use system-provided components — such as text fields and text views — you get built-in support for drag and drop.

移动端拖放交互还有不少提升空间，希望不只是停留在移动首页图标和排序列表。

---

而在 macOS 视觉被统一的趋势中，依然保留了绝大部分出色的拖放体验。在本节的最后也提到了 macOS 上拖放的注意事项：

- 考虑将内容直接拖进访达中（形成文件）。比如日历事件拖进访达后，会自动变为一个 ics 文件；Keynote 右栏图像标签下的文件信息和 Sketch 的导出预览处都可以直接拖放出来保存（Sketch 的其他拖放交互也很棒）；
- macOS 支持背景选择（background selection），可以拖放某个文件而不用激活该窗口；
- 拖动多个项目时显示数字标记（右键多个项目时也会显示计数）。这个功能相当实用，一直希望 Figma 也做一个。不过也不是尽善尽美，在 macOS 12.5.1 中，拖动显示的数字标记会因缩放和鼠标重叠，不清楚是否为 BUG。

![DD Test.png](Scenes%20Weekly%20%2368.assets/DD%20Test.png)

{上图：拖动多项目时，只有移到某些不可拖放的位置时才会正常显示数字标记}

- 可以考虑改变指针外观，来暗示拖放内容后会发生什么；
- 选择和拖动尽量使用同一个交互；

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/drag-and-drop)

---

# 摘录

这周看过的一些——

> There is a sense in which a certain amount of regulatory fines and congressional hearings and shareholder lawsuits are a cost of doing business for big tech companies: They can be expensive and annoying and one tries to minimize them, but you can’t expect to escape them entirely, or worry too much about them when they happen.

—— Matt Levine **-**  *[Musk Cancels Twitter Deal Some More](https://www.bloomberg.com/opinion/articles/2022-08-30/musk-cancels-twitter-deal-some-more)*

---

# 继续

**DreamStudio 更新**：[上期](https://designscenes.zhubai.love/posts/2175894992768299008#:~:text=%E6%B3%A8%E5%85%A5%E4%B8%8D%E5%B0%91%E7%94%9F%E6%9C%BA%E3%80%82-,DreamStudio,-%E5%B0%B1%E6%98%AF%E5%88%A9%E7%94%A8%E8%AF%A5)我对 DreamStudio 的介绍非常草率，应该说 95% 的问题是我对描述文本（prompt）没上心，而且没有多次用上 Seed 迭代图像。在看了[这个](https://twitter.com/wbuchw/status/1563162131024920576) Photoshop AI 辅助插件 [1] 的工作流后，我回去又试了试，调高了分辨率，使用了默认的 k_lms 采样（看着最顺眼），最后以 2802441179 种子生成了一幅不错的图像。

[1]: [Alpaca 官网](https://www.getalpaca.io/)正在申请注册中。

![2942356774_some_different_types_of_houses_on_the_mountain_which_has_many_trees__fog__cloud__Studio_Ghibli__anime__colorful__highly_detailed 2.png](Scenes%20Weekly%20%2368.assets/2942356774_some_different_types_of_houses_on_the_mountain_which_has_many_trees__fog__cloud__Studio_Ghibli__anime__colorful__highly_detailed%202.png)

{上图：山中村落，带着云彩和少许雾气。有裁剪。描述文本：some different types of houses on the mountain which have many trees, fog, cloud, Studio Ghibli, anime, colorful, highly detailed}

生成的该图像 Seed 为 2942356774，可以继续使用。我在隔壁 MidJourney 里使用相同描述文本试了下，~~不过刚好宕机了，~~如下图，风格很 “MJ”。

![fenx_some_different_types_of_houses_on_the_mountain_which_have__336c6602-861c-4d27-965c-95d5497578ae.png](Scenes%20Weekly%20%2368.assets/fenx_some_different_types_of_houses_on_the_mountain_which_have__336c6602-861c-4d27-965c-95d5497578ae.png)

{上图：相同描述文本，经过几次变体和升级放大后得到的图像。设置参数 --v 1 --q 2 -}

DreamStudio 尚不支持比 1024*1024 更高的分辨率，所以细节有限，显得没有 Midjourney「震撼」，Upscale 需要额外的算法配合（比如 [txt2imghd](https://github.com/jquesnelle/txt2imghd) 就使用了 [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN)，很吃 VRAM）。但其背后的 Stable Diffusion 更大的能力在于 img2img，用寥寥线条的草图配合描述文本精确地控制构图，这是 DALL·E 2 也暂时无法做到的。

→ 在 [DreamStudio](https://beta.dreamstudio.ai/) 体验 Stable Diffusion

→ 在 [Replicate](https://replicate.com/stability-ai/stable-diffusion) 体验 Stable Diffusion

→ 在 [M1/2 Mac](https://replicate.com/blog/run-stable-diffusion-on-m1-mac) 体验Stable Diffusion

→ 在 [Hugging Face](https://huggingface.co/spaces/huggingface/diffuse-the-rest) 体验 Stable Diffusion

→ 在[本地网页](https://github.com/hlky/stable-diffusion-webui)上体验 Stable Diffusion

> 💡 拓展：[4.2 Gigabytes, or: How to Draw Anything](https://andys.page/posts/how-to-draw/)

> Andy 介绍了使用 Stable Diffusion 合成图片的流程。

> 💡 拓展：[DALL·E: Introducing Outpainting](https://openai.com/blog/dall-e-introducing-outpainting/)

> OpenAI 介绍了 DALL·E 新的边界拓展功能，同样需要描述文本支持。

---

4、上个月 29 号 **mimic**（ミミック）公布，引起了巨大的反响。Mimic 是 RADIUS5 的诸多 AI 项目之一，在 beta 测试时使用15-30 张二次元人像，便可生成相近画风的人像。

![截屏2022-09-03 14.46.13.png](Scenes%20Weekly%20%2368.assets/%E6%88%AA%E5%B1%8F2022-09-03%2014.46.13.png)

{上图：mimic 首页展示由某位画师的作品生成的AI 图像}

但不像其他图像 AI 受大多数人的欢迎 [2] 那样，mimic 的反响大多为负面，鲜有[支持者](https://twitter.com/gamecast_blog/status/1564266395764162562)。

- Mimic 的主要领域是二次元，插画的个人差异化明显。很多画师之间的区分度依靠的就是「画风」；
- Mimic 没有反哺创作者。虽说是为创作者服务，但实际上大家不需要这样只能辅助生成头像的工具，TA 们的工作流中更需要优化笔画和笔刷等实际的因素；
    - Mimic 目前只能根据脸部特别生成近似图像，不支持身体、背景等；
- 最重要的版权问题。Mimic 在上传页面已有明显的版权提示，仅支持创作者上传自己的图像，但这个功能没有做任何判断，单纯的提示而已。法律风险的乌云依然挥之不去。特别当这个行为危及到一些画师自身职业时……毕竟之前人为抄袭图像的维权已经很累了。
    - DALL·E 2 和 Stable Diffusion 都使用了大量非公共领域的图片训练数据，而这种争论从 [GitHub Copilot](https://github.com/features/copilot) 时就开始了，「实用派」与「伦理派」讨论了一年多直到 Copilot 以 $10/month 推出时都没有结果。在立法完善之前，连判决先例也少有参考。

[2]: 一些艺术家讨厌现有图像生成 AI。有人拿 Midjourney 生成的画作，使用了 Gigapixel 放大器，获得了 Colorado State Fair 的 Digital Arts/Digitally Manipulated Photography 组别一等奖，详见[该事件回复](https://twitter.com/GenelJumalon/status/1564651635602853889)。

目前 mimic 全部机能停止，discord 群也关闭。甚至还有人去网暴帮助 mimic 参加测试的画师😓（[详见](https://twitter.com/illustmimic/status/1564423199009701888)）。最近图像生成领域飞速发展，mimic 是与传统职能碰撞最激烈的一次。回溯  19 世纪，摄影其实也受到了当时[艺术家的鄙夷](https://daily.jstor.org/when-photography-was-not-art/)。

→ [mimic 官网](https://illustmimic.com/zh/)

---

5、Microsoft 和 Adobe 的关系，可能[早在排版领域](https://www.thetype.com/2016/09/10968/#more-10968:~:text=%E8%A2%AB%E6%8B%92%E7%BB%9D%E7%9A%84%E5%BE%AE%E8%BD%AF%EF%BC%8C%E9%A9%AC%E4%B8%8A%E8%BD%AC%E5%90%91%E4%BA%86%20Adobe%20%E7%9A%84%E6%80%80%E6%8A%B1)走在了一起。随着 Windows 系统的市场普及，两者关系更加紧密。直到 Figma 的出现，Adobe 的「宠幸地位」遭到挑战。在去年的福布斯一篇对 [Figma 的报道](https://www.forbeschina.com/entrepreneur/56806#:~:text=%E7%94%A8%E6%88%B7%E8%AD%A6%E5%91%8A%E8%AF%B4%EF%BC%8C-,%E7%94%B1%E4%BA%8E%E6%80%80%E7%96%91%E5%85%8D%E8%B4%B9%E5%B7%A5%E5%85%B7%E7%9A%84%E5%8F%AF%E4%BF%A1%E5%BA%A6,-%EF%BC%8C%E8%BF%99%E5%AE%B6%E7%A7%91%E6%8A%80)中，我们了解到 Figma 走向付费的推手正是 Microsoft。

更具体的情况是，微软 2016 年收购了移动应用开发平台 Xamarin 的几个月，其中组内的一位高级设计师 Vančura 对共享设计组件好奇而先用起来，然后安利给了设计主管 David Siegel。在线协作方便地解决了 Sketch 的共享问题，但早期 Figma同样有很多问题，Xamarin 团队便成了 Figma 的大量反馈方。

2017 年 Vančura 去 Microsoft 总部出差时，向还在使用 Ps 和 Ai 的团队展示 Figma。这一年，Dylan Field 在 Figma 旧金山总部接待了 Microsoft 公司设计VP Jon Friedman，他问 Friedman 微软为什么不想免费用 Figma。对方答道：

> ″’Look, **we’re all worried you’re going to die as a company.**”

> “We can’t spread it inside Microsoft as a company even though we like it, because you’re not charging.”

大意是，你们 Figma 可别说没就没了啊，所以赶紧收费吧，这样我们就可以走正式渠道引入你们 Figma 了。

2018 年 Siegel 成为开发者服务业务的主管，开始更广泛地宣传 Figma。如今 Microsoft 在Figma 部署上每年花费数百万美元。Figma 为 Microsoft 定制了最高级别的企业版，还增加了对 Xbox 手柄的支持等等功能。我有些怀疑 Figma 现在[收费模式的 dark pattern](https://michalmalewicz.medium.com/figma-is-using-dark-patterns-to-charge-you-more-4f04b0537f43) 背后是微软的需求……

![GAMEPAD.png](Scenes%20Weekly%20%2368.assets/GAMEPAD.png)

{上图：Figma 中原型交互动作中，可选择使用手柄键位触发}

→ [原文](https://www.cnbc.com/2022/08/25/figma-growing-inside-microsoft-testing-longtime-deal-with-adobe.html)

---

6、汉仪字体（301270）于八月的尾巴（31日）在深交所创业板上市，作为国内字库第一股，汉仪 IPO 之路也不是那么一帆风顺。

![资金用途.png](Scenes%20Weekly%20%2368.assets/%E8%B5%84%E9%87%91%E7%94%A8%E9%80%94.png)

{上图：招股书上汉仪募集资金运用}

深交所早在 2020 年年末便受理了汉仪第一份招股书，对于我们吃瓜群众来说，汉仪的招股书可以让大众一窥国内字库公司的盈利手段：

- 字库授权；
- 互联网平台授权；
    - 主要是QQ，腾讯内部还开发了「字体结算系统」；
    - 国内手机厂商主题字体；
- 品牌定制字体服务；
- 视觉设计……比如电影海报字体设计；
- IP 联名产品服务（字体赋能！）；

![截屏2022-09-03 20.07.43.png](Scenes%20Weekly%20%2368.assets/%E6%88%AA%E5%B1%8F2022-09-03%2020.07.43.png)

{上图：汉仪视觉设计服务示例。除了海报还有一些公司定制的画册、周边等工作，「来者不拒」}

→ [查看招股书更多信息](http://static.cninfo.com.cn/finalpage/2022-08-23/1214356608.PDF)

---

7、一些简单的讯息：

7.1、Sriram Krishnan 搜集了一些政商界泄露出来的[内部备忘录](https://sriramk.com/memos.html)。

7.2、Twitter 正在测试[编辑推文](https://blog.twitter.com/en_us/topics/product/2022/twitter-new-edit-tweet-feature-only-test)功能，之后开放给 Twitter Blue 订阅者，在发布内容 30 分钟内可更改数次推文。微博在强监管的背景下，编辑功能倒没掀起过风雨。但 Twitter 涉及选举和 Musk 这样的「巨魔」，还有欧洲[监管的压力](https://www.wired.com/story/eu-opaque-policy-making-dsa/)下， 很难做。但好在终结了多年来的「纸上谈兵」，落到实处。

7.3、Meta 的 [Widely Viewed Content Report](https://transparency.fb.com/zh-cn/data/widely-viewed-content-report/#removed-content) Q2 中，在 Facebook 美国地区 Feed 中浏览次数最多的链接是 tiktok.com，哈哈。另外第 2 和第 4 名都是 spam 链接🫣。Meta 标识该排行侧重于 Facebook 外部链接排名展示。

7.4、来自 Twitter 营销团队的广告小贴士：

- 营销事件日历必备；
- 一年一度的活动可以参考上一年 hashtag 寻找灵感；
- 脱颖而出的视觉很重要；
- 视频广告的最佳展示时间在6-15秒这个区间；
- 推文尽量简洁，50-100 字左右；
- CTA 元素很重要；

→ [更多](https://www.socialmediatoday.com/news/twitter-provides-new-tweet-ad-tips-ahead-of-the-holiday-marketing-push/630336/)

7.5、Twitter 中止了想要依靠成人内容盈利的想法，因为公司没有能力过滤儿童色情虐待内容。[详见](https://www.theverge.com/23327809/twitter-onlyfans-child-sexual-content-problem-elon-musk)。

7.6、[Accessibility Not-Checklist](https://not-checklist.intopia.digital/)，又一个无障碍设计 check list。

7.7、蒙纳（Monotype）收购了 Berthold 字库，后者以 [Akzidenz-Grotesk](https://www.bertholdtypes.com/font/akzidenz-grotesk/proplus/) *字体而知名。*

7.8、Nvidia 市场趋势分布。可以看出「臭打游戏」的一直是 Nvidia 的第一市场（看那个折线，哈）。大概在 2017 年后，数据中心需求逐渐上升。联想到最近高端图形卡的出口断供，呃……

![21453bae-aa78-4cc8-b1e1-00471746e658_1700x1153.png](Scenes%20Weekly%20%2368.assets/21453bae-aa78-4cc8-b1e1-00471746e658_1700x1153.png)

{上图：Nvidia 自 2015 年的市场趋势分布}

→ [图源](https://www.libertyrpf.com/p/320-lots-of-thoughts-on-nvidia-q2)

7.9、看到 Microsoft 有 King，EA 有 Glu Mobile，Take-Two 有 Zynga，Nintendo 早已深耕手游多年，Sony（SIE）逐渐坐不住，也开始动手游心思。于是 Savage Game Studios [加入了 PlayStation Studios](https://blog.playstation.com/2022/08/29/welcoming-savage-game-studios-expanding-our-community/)。该工作室目前尚无任何作品。

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

![IMMO.png](Scenes%20Weekly%20%2368.assets/IMMO.png)

{上图：游戏 IMMORTALITY}

IMMORTALITY 是 Sam Barlow 的第三部 FMV 游戏。Barlow 以 [Her Story](https://store.steampowered.com/app/368370/Her_Story/) 知名，随后在 [Telling Lies](https://store.steampowered.com/app/762830/Telling_Lies/) 折戟（开局有着不俗的媒体评分，但是玩家评分很差，[包括我](https://steamcommunity.com/id/fenxer/recommended/762830?snr=1_5_9__402)）。Telling Lies 在于 Barlow 设置的玩家目的地是一个质量很差的狗血伦理剧，操作繁琐，没有惊喜。IMMORTALITY 改善了 Telling Lies 的一些弊端，专注于 FMV 叙事解谜，虽然也有些麻烦，但也有意外之处。

IMMORTALITY 具体玩法是，观看一小段视频，你可以点击视频里很多「热区」（人物、物体），来跳转到该「热区」出现的另外一个视频。就这样在不断的跳转中，戏剧交织着戏剧，去解开隐藏在这三部电影后的真正故事。而在跳转的过程中的自动形成的蒙太奇，给玩家一些探索感和喜剧感，这点是我感觉到的有趣之处。

IMMORTALITY 时间不长，10 小时以内肯定能通关。[媒体评分](https://opencritic.com/game/13590/immortality)夸张地高达 92 分，我个人觉得没有这么高，但 80+ 分是有的。

→ [游戏获取](https://store.steampowered.com/app/1350200/IMMORTALITY/?curator_clanid=4777282)

---

# 映像

现实拟像放映——

![Alcova-Kitchen-for-Cooking-ChmaraRosinke-IMG_5277.jpeg](Scenes%20Weekly%20%2368.assets/Alcova-Kitchen-for-Cooking-ChmaraRosinke-IMG_5277.jpeg)

{上图：NPK01 模块化厨房}

[Chmara.Rosinke Studio](https://chmararosinke.com/NPK01)

---

# 温故

→ [Scenes Weekly #19](https://mp.weixin.qq.com/s/MXedICedQ4TIBTcXbx3kog)

- iOS15 Beta 6 中，Safari 改动开始妥协
- 文字的高对比度并不总是代表易读
- 数据可视化的 20 条建议
- Hal Finney 28年前的 NFT 预测
- Obys Agency 栅格设计网页
- 哈巴狗内容社区 Moopers 标识
- Unix-like 内核 SerenityOS
- Figma Quick Actions 可以直接运行插件
- 8chan 创始人 Fredrick Brennan 谈 Twitter 新字体 Chirp
- 鉴别照片 Ps 痕迹的 Sherloq
- 用 AppleNeuralHash2ONNX 模拟Apple NeuralHash 模型输出

---

喜欢本文的话，欢迎分享、订阅。

第 67 期请[在此查看](./Scenes Weekly #67.md)。

本次封面使用了 M PLUS 2（上）和 EB Garamond（下）字体。灵感来自 POOLSUITE 的 [GRAND LEISURE](https://grandleisure.org/) 项目。