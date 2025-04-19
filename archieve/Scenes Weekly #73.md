# Scenes Weekly #73

2022-10-17

\> 设计视角下的世界——

第 72 期请[在此查看](./Scenes Weekly #72.md)。

本期出现：

- iPhone 14 Pro 个人体验
- Figma 重塑 Find and Replace
- 关于「评分」的思考
- 重读HIG（十三）
- 多元化和包容性背后的偏执
- WeLM 预训练语言模型试玩
- 其他：COLLINS 与 Figma 合作、Modern Design for Wikipedia、图解Stable Diffusion 的原理、Prompt 生成器、VirtualBox 更新到 7.0、Obsidian 推出 1.0、已编辑推文做作品集、MrBeast 的六人缩略图团队、Facebook关闭 Bulletin、Kilogram、生活大爆炸和谐片段趣闻

如有格式异常建议点击最上方「在浏览器中访问」。

---

不写 newsletter + 没有工作 + 假期 = 与世隔绝，十月份的前十天便这样过去了，比模拟离职还有点过分。

Issei 的「[MonoGoto](http://monogoto.ryouissei.com/)」月刊因忙碌也改为了不定期更新，他提到「资金来源对创作者的支持确实很重要」。我比他晚开始 newsletter 一个月，也在几个月前就开始考虑 Design Scenes 的收费计划落地。[第58期](https://designscenes.zhubai.love/posts/2153040612868980736#:~:text=%E9%A1%BA%E5%8A%BF%E5%85%AC%E5%B8%83%E4%B8%80%E4%B8%8B-,%E7%9B%AE%E5%89%8D%E7%9A%84%E8%AE%A1%E5%88%92,-%EF%BC%9A%E6%9C%AC%E9%80%9A%E8%AE%AF%E7%9F%AD%E6%9C%9F)时我表态不会去做付费墙，年轻设计专栏的转化率一定比我的半藏爆头率还低，而模式的改变却带来数倍压力，理性与感性上都是对我很不利。我已经有一个实验性的想法，还在整理规则，虽然听起来很荒谬，但走错路也没什么惩罚。

最后依然欢迎上周和上上周的新订阅者，感谢所有订阅者的支持🤠

---

# 一日不见

1、本以为中下旬才会发货的 iPhone 14 Pro 在国庆期间提前到手，用了一周后最主要的感受是比起四年前的 iPhone XR 流畅太多，比如再也不用提前一段时间打开微信的北京健康宝扫码。产品如果都以新机型为体验标准出发的话，几年后又得再受折磨。

关于灵动岛的一个问题是，以往都不会去在意的刘海，现在需要经常盯着。因为很多信息都会在那里呈现而不是全屏或者底部弹出 Sheet，这样反而强化了刘海的存在感。虽然 Apple 把感叹号做成了胶囊，但是……岛就在那里。我原以为网上那张流传的强光下灵动岛本体多少带点黑，实际上发现它比想象的还要更轻易看到本体构造。但可以预见的是，我的刘海认知心智正在被这手机改变——连这东西都能熟悉，我可能已经「百毒不侵」了。

![IMG_7050 大.png](Scenes%20Weekly%20%2373.assets/IMG_7050%20%E5%A4%A7.png)

{上图：拿 iPhone 13 在晚上室内灯光条件下，以人眼大致角度拍摄 iPhone 14 Pro}

我入手的是暗紫色，这个倒是很满意。大学时用的 [Xperia Z2](https://regional.sony.com.hk/product/apps/product/simplePage.do?modelCode=_M038782&lang=zh) 是亮紫色，现在依然摆在书架上。

另外更换 iPhone 的唯一理由是之前 iPhone XR 买的 64GB 版本，几年下来存储空间极度不够用。如果不是刚需的话，我可能也会跳过这一代。

---

2、Figma 插件 [Find and Replace](https://www.figma.com/community/plugin/735072959812183643/Find-and-Replace) 的作者 Jackie Chui 加入 Figma 后，着手把这个功能融入 Figma 中。大部分时候我们设想的查找替换功能都是一个「小功能」，就像 macOS 自带的重命名一样小巧好用。微软 PowerToys 中 [PowerRename](https://learn.microsoft.com/zh-cn/windows/powertoys/powerrename) 工具扩展了查找替换功能，但依然是工程师角度——瞧瞧那么大的窗口。

![powerrename-menu.png](Scenes%20Weekly%20%2373.assets/powerrename-menu.png)

{上图：Windows 11 中PowerRename 窗口截图}

就像上次[复制粘贴功能](https://www.figma.com/community/file/1019677205098431673)一样，Figma 这次也本着要做就做好的心态，为查找替换定下三个原则：

- 敏捷，轻便
- 丝滑，特别是在不同画板间切换时
- 和其他应用的体验相似（比如浏览器），不会有门槛

接着文中说明了以下几点衍生的逻辑：

- 搜索结果包括哪些元素类型？
- 多个搜索结果的切换顺序是什么？
- 当前视界里显示多少元素？
- 视界如何切换？
- 有些人喜欢 ⌘F 后按回车键切换到下一个搜索结果，原本回车键是深入下一图层的，该如何区分和取舍？
- ……

这其实也在启发我们，如果不深入到实际生产流程中，一些产品批评只停留在表面而很难触及根本。但对于查找和替换的切换我有些疑问：

![F&R.png](Scenes%20Weekly%20%2373.assets/F&R.png)

{上图：在同一 Figma 草稿中搜索同一关键词}

如上图所示，我在`查找`关键词 curve 时，显示的是包括文字图层在内的所有结果。但是点击右边设置图标切换到`替换`功能时，却发现只能替换文本图层。脑筋急转弯来了，Replace Layer Name需求在这里不支持，因为已经有了 Rename 功能（⌘R）。但搜索结果又不支持多选，导致`查找`后的结果只能查看。我不知道这是不是个人向需求，但确实是我的直觉和经验。

文章的最后提到「匹配大小写」也有很多细节设计，比如下图匹配规则：

![c132f55e73c9db307ae91d0b2710585956154628-1600x655.png](Scenes%20Weekly%20%2373.assets/c132f55e73c9db307ae91d0b2710585956154628-1600x655.png)

{上图：Figma 取消了匹配源大小写规则而是自立新规则，能看出替换词的形式权重更高}

慢工出细活，**Figma也在积极打造设计上的壁垒**。

→ [原文](https://www.figma.com/blog/behind-the-feature-find-and-replace/)

> 💡拓展：作者 [Jackie Chui](https://twitter.com/jackiechuichui) 还收到了Figma 官方的[下架请函](https://twitter.com/jackiechuichui/status/1578167715197751296)。虽然这次都是自己人，但不排除之后Figma 会吸收更多社区优秀插件……所以什么时候把字体选择改改呢？

---

3、Figma 在 Config2021 提出 Nothing great is made alone 的标语，最近发现是由 COLLINS 操刀，以动画形式幽默地传达了协作的重要性。COLLINS 曾为 Medium 设计过新的品牌标识，也为 Robinhood 服务过，将一些复杂金融概念融入漂亮的插图。

![截屏2022-10-14 17.15.12.png](Scenes%20Weekly%20%2373.assets/%E6%88%AA%E5%B1%8F2022-10-14%2017.15.12.png)

{上图：协作构建巨石阵}

→ [更多动画](https://www.wearecollins.com/work/figma/)

---

4、自 2000 年以来，Tom Sietsema 一直在为《华盛顿邮报》撰写美食评论。他在 2003 年引入了评星制度（0-4星级），向读者更直观地展现他对一家餐厅服务、氛围和食物的看法。

- 0 星代表就餐体验很差
- 1 星代表就餐满意（satisfactory）
- 2 星代表很不错（good）
- 3 星代表很优秀（excellent）
- 4 星代表最好的（superlative）

但自从 COVID-19 流行后，Sietsema 暂停了评分，理由是疫情期间许多餐厅只开放外卖，即便重新开放堂食后也存在疫情影响的人员配备问题，不能作为评分标准。Sietsema 重新思考了评分机制，他回想到许多人曾对他说过「我会无视低于三星级的餐厅评论」类似话语，但其实也有很多一、二星级的优秀餐厅可供选择。是时候抛弃评分了。

→ [原文](https://www.washingtonpost.com/magazine/2022/10/03/restaurant-reviews-star-ratings/)

而所谓的评分，其实只是个体或群众对该事物的期望表现，而非体现事物的质量评价。这是一种相对的后验，是事物与公众对话后的结果。但其实大部分社区和产品都没凸显这里面的相对性，在那里评分是社区表达欲与沟通的节点，需要调动社区成员情绪，使社区变得「丰富」但又容易走向极端。几年前 Netflix 想清楚了这点，取消了评分，改为点赞/踩，显示匹配账户数据的百分比，极度个人化。

说起 Netflix，他们公布了带广告套餐，除了享受基础套餐的所有权限，视频清晰度也提到了高达 720p 😲。广告分布在影片播放前和中间😑，长度15-30s，平均每小时4-5 分钟广告时长，每月 6.99 美元😅，比 hulu 低 1 美元。

→ [公告原文](https://about.netflix.com/en/news/announcing-basic-with-ads-us)

---

# 重读HIG（十三）

本节是重读 Human Interface Guidelines 系列连载第十三期，目的为温故知新和跟进新内容。 为避免篇幅过长，不会一次发布太多，之前内容已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上。

## 图表（Charting data）

图表这一节是最近新添加的，因为 [SwiftUI 框架](https://developer.apple.com/documentation/charts)中新加入了 Charts 结构。但图表设计在 iOS 等系统中都存在已久。

- 只是当做信息浏览的话，并不是所有数据都需要用图表（chart）来体现；
- 保持图表简洁，不用把一次性把所有信息都显示出来。而是逐渐地、交互地体现数据之间的关系；
- 关于图表的无障碍方面，Swift 框架的图标支持 VoiceOver 朗读图表标题、描述和单项（XY轴上的）内容和标签等信息，[后面](https://developer.apple.com/design/human-interface-guidelines/components/content/charts#enhancing-the-accessibility-of-a-chart)会说明编写建议；

HIG 中对图表的定义解构为四个方面：

- Marks（条状、线状、点状等等图形元素）
- Axes（轴，数据框架）
- Descriptions（图表描述，使人易于理解）
- Interaction（通过交互深入探索数据）
- Color（配色，使图标个性化，增加对比度）

多种多样的图形和属性结合，派生出了丰富的图表形式。

![charts.png](Scenes%20Weekly%20%2373.assets/charts.png)

{上图：WWDC22 视频中举例的 8 种类型图表}

一般来说使用常见的图表即可，像是柱状图和折线图都非常直观。使用比较新颖的图表结构时，要予以解释。比如 iOS 中的健身记录圆环。

![截屏2022-09-28 17.49.15.png](Scenes%20Weekly%20%2373.assets/%E6%88%AA%E5%B1%8F2022-09-28%2017.49.15.png)

{上图：股票应用和健身记录中的图表}

具体设计图表时，保持图表配色的一致性（尽可能彰显品牌）和连续性也是一个不简单的问题。作为仅介绍 Pattern 的一章，关于数据图表暂时说到这里。同样本节也建议观看结尾的 WWDC 视频。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/charting-data)

> 📬 回溯：[An interactive guide to color & contrast](https://colorandcontrast.com/#/)

## 协作共享（Collaboration and sharing）

Apple 的办公全家桶上线协作功能已有数年，今年大幅更新了协作功能的 Share Sheet，而且也把这部分内容新加入了 HIG 中。

![Collaboration and sharing.png](Scenes%20Weekly%20%2373.assets/Collaboration%20and%20sharing.png)

{上图：Apple 跨设备协作共享流程的生命周期}

值得一提的是，这次 HIG 里的内容是和信息应用（Message app）一起绑定拿出来说的，仿佛没了信息应用就不能协作一样……

HIG 建议：

- 将共享按钮放在方便的位置容易使用，比如 toolbar；
- 用简短的话来说明分享权限；
- 提供一个简化的分享流程；
- 协作开始后立即显示相关功能按钮和状态；
- 默认不展示过多的自定义分享操作；
- 如有必要，可以自定义分享标题，使用 CloudKit 除外；
- ……

想要了解更多的话，还是推荐看 WWDC 视频讲解，具体得多。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/collaboration-and-sharing)

---

# 摘录

这周看过的一些——

> Designer Antonio Carusone has had a similar experience. "Recently, I've given up on Instagram," he says. "I was posting there daily and saw little growth and engagement. The funny thing is, now that I've stopped, I'm growing in followers: what a weird, broken platform! Nowadays, I'm focusing instead on Twitter, where I use Typefully to plan my tweets, and I'm seeing nice results."

> Others, meanwhile, are pivoting to Facebook. "I get more orders and interaction on my Facebook business page than on Instagram, which is dire," says jewellery designer Lindsay. "With Stories and Reels, folks just mindlessly scroll rather than interact. Maybe Facebook is doing better for me because I'm from a small community and locals know my business."

—— KATY COWAN - [Is social media for self-promotion over? Creatives reveal their honest thoughts](https://www.creativeboom.com/tips/is-social-media-for-self-promotion-over/)

---

# 如三秋兮

5、在[第34期](https://designscenes.zhubai.love/posts/2082020467652382720#:~:text=4%E3%80%81-,Modern%20Design%20for%20Wikipedia,-%E6%98%AF%E4%B8%80%E4%B8%AA%E6%B5%8F%E8%A7%88)介绍过 Modern Design for Wikipedia 这个浏览器插件，可以让维基百科的页面更加清爽。作者最近又开发了 Modern for Hacker News 插件，让 Hacker News（HN）页面焕然一新。

![web_screen_2-7990a2ac063e0a593867bba4a838981d4b20e979dfc91751ab05f7fe2aa6e4d8.jpeg](Scenes%20Weekly%20%2373.assets/web_screen_2-7990a2ac063e0a593867bba4a838981d4b20e979dfc91751ab05f7fe2aa6e4d8.jpeg)

{上图：安装 Modern for Hacker News 后的 HN 首页}

除了页面排版重设计，作者也加入了很多新功能，比如历史浏览，而且把常用的搜索框挪到了顶部常驻，太棒了。不过 upvote 不知为何挪到了右边，Infinite Scroll 脚本也失效，都是小问题。

→ [立即使用](https://news.ycombinator.com/news)

---

6、Axios 也好，Bloomberg 也好， 他们推送的游戏专栏比起具体的游戏推荐，更关注游戏业界的一些涉及「人」的新闻，比如之前就连续报道了多期动视暴雪的内部文化问题。包括 Black Lives Matter 事件，在企业社会媒体和舆论的多元化和包容性（D&I）谴责时，都会立即做出一些表态，比如立即提拔XXX的职位，并会优先考虑女性和有色人种晋升。我一直有个疑问，为什么前提没有建立在相同工作能力的基础上去谈论这件事。

Jason Mansfield（化名）在 2021-2022 年间是微软 AI 部门经理，他披露了微软内部 D&I 文化的畸形走向。微软员工每年要 “Connect” 几次，就是写出未来几个月的待办事项以及如何执行，需要审批。然而核心优先事项并不是像微软企业愿景那样让地球上的人过得更好，而是需要考虑多元化和包容性。

![8b6c8099-742c-4df2-aa07-7fc5c0adfd5d_2684x786.png](Scenes%20Weekly%20%2373.assets/8b6c8099-742c-4df2-aa07-7fc5c0adfd5d_2684x786.png)

{上图：D&I 作为核心优先事项，屏摄图}

D&I 可以理解，Mansfield 继续专注于做产品。但没过多久他收到了公司 VP 发来的邮件，要求所有经理和一定级别的员工公开分享个人 D&I 计划。Mansfield 了解到仅仅是承诺不够的，D&I 需要具体的行为体现，比如：

- 雇佣「多元化」的求职者；
- 提拔「多元化」的员工；
- 参加一个「文化俱乐部」；
    - 这个俱乐部会组织演讲、观看电影和分享书籍，主题是社会正义和歧视。

Mansfield 作为部门经理被告知，在美国企业招聘时要：

- 至少面试 1 名非裔、拉丁裔、西班牙裔、黑色人种的美国求职者
- 至少面试 1 位女性求职者

在内部提拔方面，Mansfield 曾收到 HR 部们的突然通知，没有前后文的询问他是否考虑推荐一个下属晋升。在后续通话中 Mansfield 了解到HR 正在审查这些「多元化」的员工，并需要确保这些员工是否已被经理「考虑过」。

D&I 政策带来的如此偏好，并未在 HR 部门外部讨论过，这可能会打击一些真正在做实事的员工——无论他们是否「多元化」——非多样化员工感到不公平，而多样化员工也会感到被质疑（提升是因为政策还是工作能力）。从不公到另一个不公，只有偏执变得更加「多元化」。

→ [原文](https://www.cspicenter.com/p/what-diversity-and-inclusion-means)

---

7、WeLM 是微信推出的预训练语言模型，通过100亿参数的高质量语料库训练，「它在18个中文语言任务里，效果堪比参数量是其25倍的模型。」

> WeLM没有对自然语言相关的任务做任何约束或者预置。仅通过调用模型来补全您输入的文本，可以体验或者完成各种自然语言的任务。

看了几个 demo 后发现挺有意思，WeLM 的 prompt 可体现在完整的文本中，语义更连续，让我想起了之前测试 Github Copilot 帮助写文章的事（[#CopilotNotCode](https://designscenes.zhubai.love/posts/2094753654367477760#:~:text=%E5%AE%A2%E5%88%86%E4%BA%AB%E4%BA%86-,%23CopilotNotCode,-%E7%9A%84%E8%B6%A3%E4%BA%8B%EF%BC%9A)）。官方还用 Streamlit 分享了一个 playground，于是我也试玩了一下：

![WML.png](Scenes%20Weekly%20%2373.assets/WML.png)

{上图：自由任务。输入三个模型，输出结果。默认参数}

可以看到车轱辘话说的挺好听的，就是没法纠正一些逻辑错误。

→ [网站](https://welm.weixin.qq.com/docs/)

---

8.1、Jay Alammar 详细[介绍了 Stable Diffusion 的原理](https://jalammar.github.io/illustrated-stable-diffusion/)，非开发人员也可以得到一些有趣的东西。



8.2、[Stable Diffusion Prompt Generator](https://huggingface.co/spaces/Gustavosta/MagicPrompt-Stable-Diffusion) 可以根据自然语言生成一段适应 Stable Diffusion 的描述文本（Prompt）。”META Stable Diffusion！”



8.3、免费的老牌虚拟机应用 VirtualBox [更新到 7.0](https://www.virtualbox.org/wiki/Changelog)，对于 macOS 版本，移除了所有内核扩展，改为使用 macOS 系统自身的 hypervisor 和 vmnet 服务。

> 📬 回溯：Mac 提供两个级别（level）的虚拟化支持，一是使用 [Hypervisor](https://developer.apple.com/documentation/hypervisor/apple_silicon)（VMM）技术的 Parallels、VMware 等商业虚拟机产品，是需要大量代码工作量来填充的中间软件层；二是新的 [Virtualization](https://developer.apple.com/documentation/virtualization/virtualize_macos_on_a_mac) 技术，拥有更高的级别，已支持多种关键服务，而且相当轻量化。

> —— [第60期](https://designscenes.zhubai.love/posts/2158119020283875328#:~:text=%E6%94%AF%E6%8C%81%EF%BC%8C%E4%B8%80%E6%98%AF%E4%BD%BF%E7%94%A8-,Hypervisor,-%EF%BC%88VMM%EF%BC%89%E6%8A%80%E6%9C%AF%E7%9A%84)



8.4、Obsidian 从 0.16 版本直接跳到 [1.0 版本](https://forum.obsidian.md/t/obsidian-release-v1-0-0/44873)，恭喜。等待适配主题。



8.5、[上期](https://designscenes.zhubai.love/posts/2188559536175026176#:~:text=Twitter%20Blue%20%E5%B1%95%E7%A4%BA-,%E5%B7%B2%E7%BC%96%E8%BE%91,-%E6%8E%A8%E6%96%87%E7%8A%B6%E6%80%81)介绍了Twitter 已编辑推文的状态，[@omgadamho](https://twitter.com/omgadamho/status/1580000934239031297) 利用这个功能展示 portfolio，有点想法。



8.6、一个有趣的[网页动效](https://codepen.io/Mamboleoo/pen/LYmOyEG)：把输入控件当做烟花🎆发射——



8.7、VidSummit 2022 上，MrBeast 表示他的团队里有六位专门做视频缩略图的人，为每个视频制作大约 20 个版本的缩略图。如果视频一周内点击率较低，则会更换缩略图。[→ 源](https://twitter.com/arperelli/status/1575251628982403072)



8.8、Facebook 将于 2023 年初关闭时事通讯平台 Bulletin，[毫不意外](https://www.niemanlab.org/2022/10/facebook-will-shut-down-bulletin-its-newsletter-service-by-early-2023/)。

> 📬 回溯：顺便一提 Substack 是 10% 手续费，Twitter 的 Revue 是 5%，到了 Facebook 推出的 Bulletin 干脆就不收了，创作者直接获得 100% 收益。

> —— [第12期](https://www.craft.do/s/YNdfyUwCkh91p2/b/579268A6-8249-4E79-9ED5-2F61B3756EF4/Scenes_Weekly__12#:~:text=Revue%EF%BC%8C%E7%84%B6%E5%90%8E%E6%98%AF-,Bulletin,-%EF%BC%8C%E9%83%BD%E5%BC%80%E5%A7%8B%E5%85%A5%E5%B1%80)



8.9、[Kilogram](https://vole.wtf/kilogram/) 网罗了网络上低于 1 KB 大小的图片。



8.10、The Pudding 这期整理了优酷上《生活大爆炸》和原片对比后的和谐片段，共计1个多小时。主要是还有一些双标因素……推荐[观看原文](https://pudding.cool/2022/08/censorship/)，The Pudding 的可视化一直做得很棒。

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

![hero.jpeg](Scenes%20Weekly%20%2373.assets/hero.jpeg)

{上图：守望先锋 归来的三位新英雄}

数年后重回守望先锋的感觉并不怀念，但暴雪游戏的「基本质量」还是存在的。没遇到什么手感差异问题，各种反馈项依然保留。预设职责没有让游戏好玩起来，还是快速游戏随便玩玩还是可以的，反正厌倦坐牢直接退出即可。

---

# 映像

现实拟像放映——

![5282776029_9c61df0461_k.jpeg](Scenes%20Weekly%20%2373.assets/5282776029_9c61df0461_k.jpeg)

{上图：Shipping Container Sculptures In Denver}

Photo by [Scott Beale / Laughing Squid](http://laughingsquid.com/)

---

# 温故

→ [Scenes Weekly #24](https://www.craft.do/s/YNdfyUwCkh91p2/b/71AD7DD2-745A-4F1C-A3C6-F0E45DCBEA8C/Scenes_Weekly__24)

- Figma 复制粘贴全方位更新
- Noi Grotesk 字体变换
- 使用 Accessible Palette 工具构建 CIELAB / Lab* 颜色系统
- Klim Type Foundry发布了新的巴洛克风格字体 Epicene
- Fast Company年度 Innovation by Design 公布了获奖名单
- 《黑客帝国》电影的色调公式
- 美漫对话气泡排版
- 滚石杂志 500 Greatest Songs of All Time
- 江户文字介绍
- Ben Sanders 的瓶盖艺术

---

喜欢本文的话，欢迎分享、订阅。

第 72 期请[在此查看](./Scenes Weekly #72.md)。

本次封面使用了 PingFang SC 和 SF Pro Display 字体。