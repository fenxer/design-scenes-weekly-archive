# Scenes Weekly #65

2022-08-15

\> 设计视角下的世界——

第 64 期请[在此查看](./Scenes Weekly #64.md)。

本期出现：

- iOS 16 Beta 电量百分比争议
- Cyma curves 介绍
- 重读 HIG（六）
- 利用 IMDB 制造虚拟影响力
- BlenderBot 3 对新闻业发表看法
- Google 继续抨击 iMessage
- 其他：ISO 8601 日期格式标准、网络跟踪保护介绍文档、Google 表单密室逃脱游戏、10 条 DALL·E 2 经验、Fluent Emoji 开源

本期内容较长，建议点击最上方「在浏览器中访问」。

---

综合性每周通讯的一点好处是选择性更多，只看自己想看的部分就行。

如果通讯里只保留一个栏目的话，我应该会留下每周游戏推荐。很羡慕[逆风笑](https://space.bilibili.com/2019740)的创作状态，但我并不喜欢的他的声音。

然后，欢迎上周的新订阅者。感谢所有订阅者的支持。

---

# 杂事

1、上周 iOS 16 Beta 5 的电量百分比更新引起了热议，甚至一度上了微博和 Twitter 热搜。好奇如此关注度的同時，发现我的 iPhone XR 没有获得此更新，让我有了新的困惑。这次总不能拿性能作为说辞了吧——网上的主流观点是支持的机型都有着接近 460 PPI 的屏幕。我从网上和朋友那里搜集了一下相关截图，尝试在 XR 上观察仅以 2 倍缩放大小的图——

![1670064939660.png](Scenes%20Weekly%20%2365.assets/1670064939660.png)

{上图：测试在 iPhone XR 中显示百分比电量，图片尺寸不代表实际，只能做到接近显示比例}

电池图标确实比之前大了一圈，字号 11 pt，直接替换原有电池图标便是上图效果，可以看到确实和右边缘贴的比较近，但实机并不会出现看不清数字、数字模糊等状况。

iPhone 这几年随着物理屏幕的更迭，对于「刘海」（notch）所在的状态栏也有设计上的微调。

![1670064941268.png](Scenes%20Weekly%20%2365.assets/1670064941268.png)

{上图：不同宽度下的状态栏图标位置对比}

这些改动大都依靠于实际 notch 左右留下的空间来调整，对于实际设计界面时看不到 notch 的设计师来说却是很烦躁的问题，因为它的调整并没与遵循界面中的逻辑，而是现实中的物理逻辑。虽然大部分时候状态栏都只是几乎不变的通用组件，但是看着曾以「设计通用性」为称的 iOS 也累加起了设计债，不由心生感叹。

另一方面的争议是，电池电量在 20% 前一直是满的，反直觉。有人提出了替代方案，比如下面很多人见过的这张图：

![1670064942988.png](Scenes%20Weekly%20%2365.assets/1670064942988.png)

{上图：Twitter 用户 Mikael Johansson 给出的替代方案}

- A 方案是在数字背后加上背景，但是这样会降低文字对比度（看不清），不确定使用 vibrancy 渲染会不会更好一些；
- B 方案是给数字加上描边，印象里 iOS 没有这种文本处理方式；
- C 方案是给数字加上差值混合模式，这样会在数字和背景相遇时大幅降低易读性；

三种方案都不太理想。总之还是看 Apple 下一步是否迭代。离秋季还有一段时间，现在 beta 版的问题依然不少，尝鲜需谨慎。

---

2、本周的 [Design Lobster](https://designlobster.substack.com/p/115-curve-ball) 介绍了 cyma curves 这一建筑术语（罗马式[表反曲线](https://en.wikipedia.org/wiki/Ogee)，也用于数学、流体力学和整容）。你可能在现代的家具和屋饰装修中有看到此类流畅的曲线。

![1670064944592.png](Scenes%20Weekly%20%2365.assets/1670064944592.png)

{上图：在 cyma curves 中总有一条不可视的直线贯穿其中}

它的几何原理很简单，我在 [Euclidea](https://apps.apple.com/us/app/euclidea/id927914361) 里使用探索模式简单画了下，如下图。

![1670064946260.png](Scenes%20Weekly%20%2365.assets/1670064946260.png)

{上图：在 Euclidea 中演示两种 cyma curves }

两段曲线的弦有着不同的比例，有时需要不同的曲率的曲线衔接。上面两种使用的是「慢曲线」衔接，另一种画法是更凸起的「快曲线」。

![1670064949869.png](Scenes%20Weekly%20%2365.assets/1670064949869.png)

{上图：左边为 Slower Curve，右边为 Faster Curve }

将多个比例、曲率的曲线连接在一起便形成了一些古典家具的优雅曲线。如果遇到曲线衔接不流畅的时候，也可以链接处做额外的装饰，比如削平一小段，或者加上额外的装饰掩盖没对齐的尴尬。

→ [家具应用介绍](https://www.youtube.com/watch?v=Bqev7o-4U6o)

[Cyma Curves in Furniture Aprons](https://www.youtube.com/watch?v=Bqev7o-4U6o)

→ 曲线画法

[Draw Cyma Curves](https://www.youtube.com/watch?v=9M18Sna44EA)

→ 更多考据（推荐）

[http://www.woodworkinghistory.com/glossary_cyma_curve.htm](http://www.woodworkinghistory.com/glossary_cyma_curve.htm)

---

3、国外常用的「日月年」或「月日年」日期顺序，在不了解前后语境时，很容易误读。虽然我们说本地化设计要符合当地文化习惯，但日期格式其实是有国际通用标准的。

ISO 8601 规定了通用日期格式为「年月日」，即 YYYY-MM-DD。分隔符可以是 - / . , 空格、年月日和无分割，取决于整体的统一性。

→ 原文

[What’s the best way to display dates to international users?](https://uxpsychology.substack.com/p/whats-the-best-way-to-display-dates)

→ ISO 8601

[ISO 8601 - 维基百科，自由的百科全书](https://zh.wikipedia.org/wiki/ISO_8601)

---

# 重读 HIG（六）

本节是重读 Human Interface Guidelines 系列连载第六期，目的为温故知新和跟进新内容。 因为篇幅原因不会一次发布太多，之后会专门整理。

上周看到超人的电话亭团队有在翻译新的 HIG，包括一些图片和表格都做了汉化。翻译工作实属不易，有需要中文版的可以看看。但个人建议还是中英对照学习，翻译貌似尚未润色，且有未翻译的地方。

顺便吐槽下 Craft 的子页面居然没有独立的链接……

→ 预览

[http://www.supermancall.com/](http://www.supermancall.com/)

## 材质（Materials）

- 材质这一节，首先提到了 vibrancy 渲染。它适用于在不透明材质上突出主体内容，HIG 并未对此做详细介绍（为什么？），但在 [WWDC19 的视频](https://developer.apple.com/videos/play/wwdc2019/808/)中我们可以一窥其貌。如下图，简而言之 vibrancy 会提取背景颜色，赋予主体内容的填充具有沉浸感和可读性；

![1670064951516.png](Scenes%20Weekly%20%2365.assets/1670064951516.png)

{上图：不同背景上，使用固定颜色和 vibrancy 的对比}

- HIG 依然建议使用 SF Symbols 而不是自定的彩色图标，Apple 的设计和开发人员已经针对 SF Symbols 做了很多自适应的优化。这在后面 [SF Symbols](https://developer.apple.com/design/human-interface-guidelines/foundations/sf-symbols) 一节中会提到；
- 系统的背景层分为了语义化的四种：透明度由低到高为 Thick、Regular、Thin 和 Ultrathin（依然藏在上面提到的 WWDC19 视频中，恼），其中 Regular 为默认；

![1670064953238.png](Scenes%20Weekly%20%2365.assets/1670064953238.png)

{上图：浅色和深色模式下，四种透明度（当然透明度并不是唯一参数指标）的背景层}

- 在选择上述哪种背景层时，可以考虑：
    - Thick 层可以为上面的内容（特别是需要精细展示时）提供更好的对比度；
    - 半透明图层则可以让用户看清后方内容，提醒他们处于流程的何处（上下文提醒）；
- 在 iOS 和 iPadOS 上，vibrancy 可以选择四种层级的值。默认为最高对比度；
- macOS 上则是针对各个语义颜色分别定义其 vibrancy 版本的色值。也提供了带有透明度和模糊度特性的面板材质，分为两种模式：
    - Behind-window blending：对程序之外的背景进行取样处理。比如提醒事项、访达等应用左侧栏；
    - In-window blending：对程序内部的背景进行取样处理。比如地图应用；

→ 本节出自

[Materials - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/materials)

## 动效（Motion）

- 动效是用来传达信息的。一个动效的起始和终止状态可以帮助用户增强对交互的理解，例如 macOS 中访达窗口的最小化或关闭后触发的「神奇效果」或缩放效果动画，帮助用户理解文件夹缩小到了哪里；
- 如果一个动效没有目的就去掉它，不要为了添加而添加（原文用的就是 the sake of adding）；
- 确保界面离开动效，交互也不会出现问题。Apple 系统设置中会有「减弱动态效果」选项，用户开启后，要确保动效最弱化或者直接消除；
- 人们喜欢快速而又精准的动效，会感觉应用更轻巧，干扰更少；
- 避免在频繁发生的交互中添加动效。这一点很容易忽视，而且不光是应用程序，还广泛存在于各个电子产品中（比如《[集合啦！动物森友会](https://zh.wikipedia.org/zh-sg/%E9%9B%86%E5%90%88%E5%95%A6%EF%BC%81%E5%8B%95%E7%89%A9%E6%A3%AE%E5%8F%8B%E6%9C%83)》中的一些对话动效）；
- 本节注意事项只点名了 watchOS。WatchKit 中的动效无法自定义缓动曲线，只能使用系统默认提供的曲线。除此之外还提供了以下属性作为动效「关键帧」：
    - 对齐方向（Alignment）
    - 背景颜色（Background color）
    - 组内间距（Group insets）
    - 高度（Height）
    - 透明度（Opacity）
    - 强调色（Accent color）
    - 宽度（Width）
- watchOS 同样也允许创建图像序列帧；

→ 本节出自

[Motion - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/motion)

---

# 摘录

这周看过的一些——

> 我的一位考古学家朋友最烦的就是互联网总想给他们行业赋能。“互联网公司觉得帮助恐龙学家研究恐龙是一种施舍：你们这些老旧的行业都能用上我们这么新的技术了。” 他说。有公司曾提出用云计算合作，“云计算的用户协议是公司写的，服务说停就停。这顶多叫 ‘出租’ 能。”

—— 晚点 LatePost - 认真谈谈为什么互联网热衷说黑话

[认真谈谈为什么互联网热衷说黑话](https://mp.weixin.qq.com/s/6qkgM7PqLuUTJx2VsLXt0A)

---

# 小事

1、DuckDuckGo 告诉我们，现在的隐私牌并不好打，本通讯也提到数次 DDG 负面新闻。先前 DDG 自己开发的浏览器被曝出只允许微软的跟踪器继续运行（两者有广告上的合作关系）。尽管 DDG 一再解释微软不会分析用户行为，但仍受到了社区强烈谴责。而终于在即将到来的测试版中，CEO Gabriel Weinberg 表示会开始阻止微软的跟踪器。

看，DDG 就是这么一个为了隐私先行，而怪异举动频发的公司。但说实话我很喜欢他们的帮助文档，这些文档总是字斟句酌地尽力向你解释关于隐私 DDG 做了什么，甚至可以当做隐私百科查询参考，比如网络跟踪保护这个新页面详细介绍了第三方跟踪器、第一 / 三方 Cookie 和 CNAME 伪装等跟踪手段。

→ 新闻源

[DuckDuckGo increases protection from Microsoft trackers after community backlash](https://9to5mac.com/2022/08/05/duckduckgo-protection-from-microsoft-trackers/)

→ Web Tracking Protections

[Web Tracking Protections](https://help.duckduckgo.com/privacy/web-tracking-protections/)

---

2、[第 50 期](./Scenes Weekly #50.md)我们得知了 Spotify 上 Fake Artist 产业凭借搜索流量获得了不小的利润。最近看到 Pea Bee 介绍了又一类似怪象：利用 IMDB 职员表制造虚拟影响力。

作者在查看 2023 年即将上映的印度电视剧 [Animal](https://www.imdb.com/title/tt13751694/) 时，发现了一个陌生的面孔 Subhankar Bagchi。

![1670064955598.jpeg](Scenes%20Weekly%20%2365.assets/1670064955598.jpeg)

{上图：Anima 电视剧中 Top Cast 一栏，原作者截图}

哥们的眼神带着一丝智慧的影子，点进去还能看到他的照片和参影履历，可见他度过了忙碌的 2022 年。用 Google 搜索名字，还能发现他有单独的知识面板（knowledge panel），「一眼顶真」。

![1670064957283.png](Scenes%20Weekly%20%2365.assets/1670064957283.png)

{上图：Subhankar Bagchi IMDB 个人资料页（左 1 和 2），Google 搜索结果（右 1），原作者截图}

在原作者的深挖之下，终于发现了马脚。原来包括 Subhankar Bagchi 在内的很多人，都在使用 IssueWire 提供的 PR 稿服务。这些年轻人有着几乎相同内容的传记，被搜索引擎一一收录。他们在 IMDB 上同样在冒名制作人员，并有着丰富的资料页。最后这些资料被 Google 等搜索引擎认为是真正的有影响的人，并为之建立独立的知识面板。他们都有着一些共同的特点：

- 都参与了印度高成本大制作的电影等媒体，但都未提及具体是什么角色或职位；
- 都是 10 几岁到 20 出头的印度北部小镇年轻人；
- 都是音乐人或 Youtuber，主流媒体平台上都有自己的作品；
- 在一些网站上都有自己的传记和生平简介，内容不能说差不多，但可以说完全一致；
- 都有自己的 Google 知识面板；

后续作者还发现了一个孟加拉 Youtuber 有一系列视频教学，教你如何从零建立自己的 Google knowledge panel。讽刺的是，上述年轻人有些人是真正的创作者，在 Instagram 和 Youtube 上有着不少粉丝，并在个人简介里指向他们的 Google 知识面板链接。而欺诈者的头衔又能掩盖多久呢？

截至写下本文时，IMDB 上该制作人员资料已经恢复一些，但是 Google 知识面板依然存在。

→ 原文

[#16: The case of fake IMDb credits](https://peabee.substack.com/p/16-the-case-of-fake-imdb-credits)

---

3、在 V2EX 发现了一个用 Google 表单做的密室逃脱游戏，挺有趣。想起了两年前有人在 Figma 里利用组件切换特性做了一个密室逃脱 [Escape Room: The Mystery of Everson Manor](https://www.figma.com/community/file/899042758064025062)。

→ 我想回家了

[我想回家了](https://docs.google.com/forms/d/e/1FAIpQLSfZfcg8E0vxQsU0xM5hpowQtWHfKbYaMxjQDIdYDoiUmUGGrw/viewform)

---

4、我很少发布关于 Facebook 的信息，早早停止使用脸书服务的我落后于大部分话题背景（不看财报和新闻），改名 Meta 后更是鲜有兴趣关注。包括之前 Tom Alison [备忘录泄露](https://www.documentcloud.org/documents/22060613-tom-alisons-facebook-memo-42722)事件，这其实可以重启本通讯谈论 Facebook 的话题，但是写着写着发现自己并不太了解扎式社交网络，即便我隐约觉得 Michael Mignano 这篇「[社交媒体已死](https://every.to/p/the-end-of-social-media)」文章的分门别类有些牵强，却也无法自信地提出异议。

但是最近的 BlenderBot 3 新闻中，我觉得可以照本宣科地介绍下 Joshua Benton 这篇文章（BlenderBot 3 仅限美国地区用户使用）。Nieman Lab 一直关注着新闻业发展，所以他们整了个活，打算跟 BlenderBot 聊聊新闻行业的事。

以防有些读者不清楚 BlenderBot 3 为何物—— BlenderBot 是 Meta 推出的最新一代聊天机器人，在人格、同理心和知识层面取得了不错的进展，并且有着更长期的记忆（联系更多上下文）。Meta 虽然在偏见和冒犯言论上做了很多限制，但依然无法阻止 AI 爆粗，以至于一周后 BlenderBot 3 就变得像个疯疯癫癫的种族主义者。

另一个需要了解的是，广告行业的疲软对新闻业也有相当的影响。纽约时报的 CEO Meredith Kopit Levien 在接受 Ben Thompson [采访](https://stratechery.com/2022/an-interview-with-the-new-york-times-company-ceo-meredith-kopit-levien/#adsaudio)（付费墙注意），被问及如何看待宏观经济的下滑对广告的发展时，只能说些车轱辘话搪塞过去，也没能接住大 Ben 哥最喜欢的 #App Tracking Transparency 话题。

回到 Nieman Lab 这篇新闻，Benton 询问 BlenderBot 有什么方法能重振新闻业。BlenderBot 的答案是教育，优质新闻生产需要优质作家，优质新闻消费需要高质量读者。这个回答真是一个美妙的开局。

- Benton：在互联网兴起之前，纸媒已经赚的盆满钵满。
- BlenderBot：罪魁祸首绝对是 Craigslist（美国免费分类广告商）。
- Benton：不是 Facebook 的错吗？
- BlenderBot：纸媒在 Facebook 前就死了，Facebook 只不过加速了这一状况。
- ……

BlenderBot 会随着聊天逐渐「了解」对象，聊得越多，对话越独特越定制化。更多有意思的对话还请查看原文。

→ 原文

[Blame Craig: How Facebook’s AI bot explains the decline of the news industry](https://www.niemanlab.org/2022/08/blame-craig-how-facebooks-ai-bot-explains-the-decline-of-the-news-industry/)

---

5、Deephaven 花了 45 美元用 DALL·E 2 替换了他们所有博客文章的封面图。作为一家数据技术公司，过于抽象的文章配图会有一种疏远感，解放想象力的 AI 或许能带来不一样的一面。

![1670064959316.jpeg](Scenes%20Weekly%20%2365.assets/1670064959316.jpeg)

{上图：Deephaven 替换文章封面图前后对比}

替换的结果是成功的，但是过程却很艰辛，Deephaven 总结了 10 条：

- AI 做图让人的创作力从设计转移到描述文本（prompt）；
- 不要指望 AI 一次就能生成好图像，需要多次练习描述；
- XX 风格的描述很重要。可以出自电影、可以是[美学术语](https://aesthetics.fandom.com/wiki/List_of_Aesthetics)，也可以模仿某个著名艺术家；
- 像别人学习怎么写描述文本，比如多逛逛 [r/dalle2](https://reddit.com/r/dalle2)。[第 61 期](https://designscenes.zhubai.love/posts/2160656211648229376#:~:text=%E9%87%8E%E7%94%9F%20AI%20%E6%8A%80%E5%B7%A7%E3%80%82-,DALL%C2%B7E%202%20Prompt%20Book,-%E8%BF%99%E4%BB%BD%E6%96%87)提到的 DALL·E 2 Prompt Book 也是不错的参考；
- DALL·E 2 有时会带着水印或者迷之文字一起生成，目前对字体的处理还是弱项；
- 一些意料之外的违规内容。比如「shooting」一词，原文想表达一束光射向天空，但 DALL·E 2 会提示含有违禁词；
- 一些尺寸裁剪和后期处理依然需要设计工具，长远看 AI 配图只是融入设计中一环，并不会完全抢占设计流程；
- 想指定图片中特定的物品、颜色、数量和位置都比较困难；
- 艺术家角色不会因此消失；
- 但对图片售卖网站来说是个危机；

→ [原文](https://deephaven.io/blog/2022/08/08/AI-generated-blog-thumbnails/)

[I replaced all our blog thumbnails using DALL·E 2 for $45: here’s what I learned | Deephaven](https://deephaven.io/blog/2022/08/08/AI-generated-blog-thumbnails/)

也可以顺便看看 Jacob Martin 如何用 DALL·E 2 生成可爱的小章鱼 logo。Martin 使用 AI 一共生成了 51 张图像才得到他满意的吉祥物，一共花了 30 美元。在订阅模式水深火热的国外已经很便宜了。

![1670064961164.png](Scenes%20Weekly%20%2365.assets/1670064961164.png)

{上图：描述文本为 Cute baby octopus playing with mussels wearing a yellow safety helmet, logo, digital art, drawing, in a dark circle as the background, vibrant, cheerful, bubbles，然后经过变体得到该图}

→ 原文

[How I Used DALL·E 2 to Generate The Logo for OctoSQL](https://jacobmartins.com/posts/how-i-used-dalle2-to-generate-the-logo-for-octosql/)

---

6、上周微软开源了 Fluent Emoji，这是件好事。其中不包括商标、国旗等含有法律、政治风险的表情，但也有 1500 余个。开源的表情文件分为四种：

- 3D 图标，位图（PNG）
- 全彩图标，SVG，和 3D 图标几乎没区别
- 扁平图标，SVG
- 黑白图标，SVG

在微软的 [Figma 主页](https://www.figma.com/@microsoft)也能看到三份相应的设计文件。如此多的数量也带来了庞大的审校工作，比如 pretzel 饼干表情就发生了错位，GitHub 那边也有不少[尺寸问题](https://github.com/microsoft/fluentui-emoji/issues/34)。

![1670064962851.png](Scenes%20Weekly%20%2365.assets/1670064962851.png)

{上图：在 Fluent emoji — 3 文件中的小错误}

另外，微软那篇在 Medium 的公告文章绝对是专业的 UX 作家所写，能把一件简单的事扩展成那样谈古论今，还能灌入微软设计文化，不免啧啧称奇。

→ 原文

[Designing in the Open(Source)](https://medium.com/microsoft-design/designing-in-the-open-source-5c62be73a599)

---

7、本通讯[第 35 期](https://designscenes.zhubai.love/posts/2094753654367477760#:~:text=Google%20%E6%83%B3%E8%A6%81%E6%8E%A8%E5%8A%A8-,RCS,-%EF%BC%88%E8%9E%8D%E5%90%88%E9%80%9A%E4%BF%A1%EF%BC%89%E4%B8%9A%E5%8A%A1)提到 iPhone 中蓝绿气泡所衍生出的社会现象。当对方使用的是非 Apple 设备时，iMessage 的聊天气泡会变为绿色，而不是蓝色。绿色气泡通信使用的传统的 SMS 和 MMS 技术，没有端到端加密，也无法传输清晰的图片，无法应用 RCS 标准带来的更多便利功能。最重要的是，这促使了青少年中产生了挤压和欺凌的阶级断层。

所以 Android 在此事上数次指名 Apple 要求其改善该状况，特别是最近专门建立一个网页来阐述 iMessage 的「七宗罪」。

![1670064964696.png](Scenes%20Weekly%20%2365.assets/1670064964696.png)

{上图：It’s time for Apple to fix texting 网站截图}

在去年 Apple vs Epic 事件中，Apple 被曝出早在 2013 年就有开发 Android 版 iMessage 的想法，但是 Apple 高管们担忧系统竞争性下降而放弃开发，此举更为 Apple 蒙羞。Apple 一直未对此置评。

Android 或者说 Google 虽然是推动 RCS 的一方，看似在拯救万千青少年脱出鄙视链的鸿沟，但实则自己在 RCS 上也有不少问题。RCS 在 2007 年由某些赞助团体推广成立，各个运营商需要单独升级自家 SMS 设施，以支持 RCS 和 Universal Profile（简单理解成手机号）。由于缺乏升级动力（没公共补贴，也没啥用户需求），进展缓慢，远谈不上 RCS 标准体验。在通信业务上屡败屡战的 Google 开始鼓吹对手尚不支持的 RCS 标准，收购了当时为运营商提供后端服务的 Jibe Mobile 公司挪为己用，并自称是帮助运营商推进 RCS 标准建立，当建立完善时，Google 会将控制权交付给运营商。

彼时的 RCS 也不支持端到端加密，Google 建议大家使用 Messages 来体验谷式 RCS，但依然保留了落后的手机号码验证机制，非 SIM 卡设备无法通过验证。此举将运营商们排除在外，甚至包括自己的 OEM 盟友——三星直到 2020 年才能够让用户使用 Samsung Messages 体验 RCS（消息会以蓝色气泡表示，不是绿色，哈哈）。至于知情大众是真的厌倦了 Google 的折腾，打破了本来运营商层面的静默升级，就不要再来当小丑了。

你怎么看待这场闹剧呢？

→ 网站

[It’s time for Apple to fix texting.](https://www.android.com/get-the-message/)

→ 参考新闻

[Google’s ninth attempt at a messaging service will be based on RCS](https://arstechnica.com/gadgets/2019/06/google-ninth-attempt-at-a-messaging-service-will-be-based-on-rcs/)

---

> 我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) ([figma.com](http://figma.com))

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) (zhubai.love)

---

# 劳逸

![1670064966592.png](Scenes%20Weekly%20%2365.assets/1670064966592.png)

{上图：7x7 新谜题与完成后的样子}

Hexagonal pipes，接水管，但是六边形。由 Daria Vasyukova 开发，接水管的四边形变为六边形后，还是有些不一样的体验，难度也提升不少。同样可每日挑战。

→ 点开即玩

[Hexagonal pipes puzzles](https://hexapipes.vercel.app/hexagonal-wrap/)

---

# 映像

现实拟像放映——

![1670064968265.jpeg](Scenes%20Weekly%20%2365.assets/1670064968265.jpeg)

{上图：雪中的乌鸦夫妇}

今年的奥杜邦摄影奖获奖作品之一，作者 Ankur Khurana。

→ 查看所有获奖作品

[The 2022 Audubon Photography Awards: Winners and Honorable Mentions](https://www.audubon.org/magazine/summer-2022/the-2022-audubon-photography-awards-winners-and)

---

# 温故

→ Scenes Weekly #16

[Scenes Weekly | No. 16](https://mp.weixin.qq.com/s?__biz=Mzg3NzYwNDEzOQ%3D%3D&mid=2247484196&idx=1&sn=b6a4cdb25a8911d1b67186468ca477f3&chksm=cf213f60f856b67652cabd8e8fad8341c8a37fd3bc2a3709cb621209796e5a40a0840969e687&scene=178&cur_album_id=1830757229226950666#rd)

- Gamestop 购物体验四个问题
- Signal 捐赠交互重设计
- Steam 久违更新了移动端游戏详情页面
- 配色灵感测试工具 Happy Hues
- GitHub 新增 Cite 仓库功能
- Discord 推出 Thread

---

喜欢本文的话，欢迎分享、订阅。

第 64 期请[在此查看](./Scenes Weekly #64.md)。

本次封面使用了 SF Pro 字体。

