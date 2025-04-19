# Scenes Weekly #70

2022-09-17

\> 设计视角下的世界——

第 69 期请[在此查看](./Scenes Weekly #69.md)。

本期出现：

- The Verge 重设计背后
- 即时设计推出即时 AI 插件
- Figma 与 Adobe 杂谈
- The Follower 实验项目
- 其他：iOS 16.1 电量百分比更新、灵动岛模拟动效设计文件、Have I Been Trained、为什么播客背后的赞助都是 VPN 厂商、直观的二维码原理说明、Smart Brevity® 书籍批评、2022 年搞笑诺⻉尔奖

如有格式异常建议点击最上方「在浏览器中访问」。

---

首先谢谢 Adobe 和 Figma 给本期贡献的话题，让我等非金融精英人士也体会到了 “The Merge”，在本周小事中会稍微详谈。另外在写本文时还看到了 EVGA “[The Rollback](https://www.tomshardware.com/news/evga-abandons-the-gpu-market-reportedly-citing-conflicts-with-nvidia)” 的新闻，真是复杂的一周。

另外之后会继续调整每期内容结构，使文本量轻重有度，避免过长。否则不论是阅读还是写作都开始有压力。

欢迎上周的新订阅者，感谢所有订阅者的支持。这期也是直接开始吧。

---

# 杂事

**iOS 16.1 电量百分比更**新：[第65期](https://designscenes.zhubai.love/posts/2170801615631011840#:~:text=Beta%205%20%E7%9A%84-,%E7%94%B5%E9%87%8F%E7%99%BE%E5%88%86%E6%AF%94,-%E6%9B%B4%E6%96%B0%E5%BC%95%E8%B5%B7%E4%BA%86)提到了当时热议的电量百分比更新，市面传闻只有 460 PPI 才享有的功能如今在 iOS 16.1 Beta 中开放给了更多机型，包括 326 PPI 的 iPhone XR——就像我之前预测的那样，字体为 11pt 的 Bold 字重 SF系列。比起「刘海」更窄的机型，老式机型的新电池长度都稍微短一些。

![Battery.png](Scenes%20Weekly%20%2370.assets/Battery.png)

{上图：iPhone XR 开启电量百分比}

---

1、本周 The Verge 的重设计令人感兴趣的点在于，首页基于 Storystream 重新进行了构建。主编 [Nilay Patel](https://twitter.com/reckless) 和 Dieter 觉得发现自己使用 Twitter 的频率比自家 The Verge 还多，于是重新拿出了当年 Vox Media 发布短幅内容渠道 Storystream，以此为基础将自家报道链接、外部新闻链接、Twitter、简要、Youtube 甚至 TikTok 和 Reddit 都集中在这条时间线上——你应该感觉到了，The Verge 的「对手」不是 Bloomberg 或是 Wired 等同行，而是 Twitter——这是一个 PGC 的按时间顺序的 “Twitter”，融入到了一个老式新闻网站。

![TheVerge_Letterforms_09.png](Scenes%20Weekly%20%2370.assets/TheVerge_Letterforms_09.png)

{上图：The Verge 新标识，跳脱性和极强的特征让它注定会被「爱憎分明」}

6 年前的 The Verge 和大多数新闻网站一样，由算法驱动着页面结构。使用着粉红色的引用语，凸显 The Verge 品牌的认知。如今作为 Vox Media 旗下最流行的媒体主页，The Verge 重新思考自己的使命。

> **The internet is about conversations, and *The Verge* should be a place to find great conversations.**

- The Verge 的主页想要集中更多优秀的报道，这不免增加了跳出率。但他们认为只要新闻提要写得够好，读者是会再回来的；
- Storystream 的低门槛发布机制，方便了实时更新，不必扩写一些重复的内容，让编辑们有时间专注于更深入的原创报道；
- 新闻应该先是让读者感到有趣，而不是完成 KPI；
- Storystream 虽然保留了广告位，但是只保留原生广告，不带有编辑主观立场；
- Nilay Patel 透露了 Storystream 能为其他新闻出版商带来比 Twitter 更快速更多的流量这个「野心」；
- The Verge 换用了 Coral 评论平台，[Polygon](https://www.polygon.com/) 也在用。除了功能增加外，界面看着还有很多改进之处，比如过小的加入对话入口，全篇幅彩色字体阅读很累等等；

社交媒体崛起一度让新闻门户主页衰落，不少人因此不看好 The Verge 在主页上大动干戈。不过 RSS 依然是小众，社交媒体又被算法控制，The Verge 想成为新闻源的阅读终点，依然需要很大一个空间去容纳。

→ [官方文章](https://www.theverge.com/2022/9/13/23349876/the-verge-website-redesign-new-newsfeed-blogs-logo)

→ [Nieman Lab 的报道](https://www.niemanlab.org/2022/09/the-verge-goes-back-to-bloggy-basics-with-a-new-redesign/)

→ [Nilay Patel 采访](https://stratechery.com/2022/an-interview-with-the-verge-editor-in-chief-nilay-patel-about-building-a-destination-site/?access_token=eyJhbGciOiJSUzI1NiIsImtpZCI6InN0cmF0ZWNoZXJ5LnBhc3Nwb3J0Lm9ubGluZSIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJzdHJhdGVjaGVyeS5wYXNzcG9ydC5vbmxpbmUiLCJlbnQiOnsidXJpIjpbImh0dHBzOi8vc3RyYXRlY2hlcnkuY29tLzIwMjIvYW4taW50ZXJ2aWV3LXdpdGgtdGhlLXZlcmdlLWVkaXRvci1pbi1jaGllZi1uaWxheS1wYXRlbC1hYm91dC1idWlsZGluZy1hLWRlc3RpbmF0aW9uLXNpdGUvIl19LCJleHAiOjE2NjU4MzQ4NjgsImlhdCI6MTY2MzI0Mjg2OCwiaXNzIjoiaHR0cHM6Ly9zdHJhdGVjaGVyeS5wYXNzcG9ydC5vbmxpbmUvb2F1dGgiLCJzY29wZSI6ImFydGljbGU6cmVhZCBhc3NldDpyZWFkIGNhdGVnb3J5OnJlYWQiLCJzdWIiOiJYbkRxMW9nY1BhQnZWYXk2czR4eGpoIiwidXNlIjoiYWNjZXNzIn0.aO_tyZDlrwvGAtiWOdld9PbZd6CvoPLNjLhwEGSvwKUnCYFOLztxrxU68rpE59JaNBV35sv6MnK1Uc9ArUhHrH88Kr4ild619gv-SKoqwgInRC0urr7xoWM_6BVgGzVYadry32JXotq7nTaw15mGiLN0kvCCGM7D03uazIQBo40PrTU7pX6TrjP50hst57z2twWPG2TNgqcua712B-y5oU8PP_eBt5wrX-b67EH4wLoUzkjW6eHS5AzzTvYDqabfykPFubuMH2bLjaZqLz8AHOSyDNeaumUX2n7ujR3fvdXlxaEDO7keZ7iKORYJ-T9dmWeyUWZYkJDQ2Bx-Yv2JxA#business-ethics)

---

2、在 [Figma 社区](https://www.figma.com/community/search?resource_type=mixed&sort_by=popular&query=dynamic+island&editor_type=all)文件泛滥之时，**Artboard Studio** 官方也发布了一个文件，快速方便地实现灵动岛效果，做了很详细的说明。想做动效届 Figma 蹭热点方向是不可少的。

![Capture-2022-09-15-153015.png](Scenes%20Weekly%20%2370.assets/Capture-2022-09-15-153015.png)

{上图：Artboard Studio 灵动岛分享文件和说明}

→ [文件](https://app.artboard.studio/project/63198f17ed31dd001c34af4b/dynamic-island?objectId=0)

---

3、即时设计推出了[即时 AI](https://js.design/pluginDetail?id=6322a4ab0eededcff6ba451a) 插件，可使用中文语义描述生成 AI 图像。

![截屏2022-09-15 16.04.59.png](Scenes%20Weekly%20%2370.assets/%E6%88%AA%E5%B1%8F2022-09-15%2016.04.59.png)

{上图：插件实际使用界面}

即时 AI 调用的是 Stable Diffusion 模型，支持图文（image-to-image）和文字（text-to image），描述可用中文，像面包多的 [6Pen Art](https://6pen.art/) 一样。虽然看到即时也在尽力提供预设图片和文字，但是缺少详细调参和 Seed 依然让 AI 很难调教。

而且在国内创作环境中，还要有一定的政治敏感性来把控 AI 生成……比如百度的 [ERNIE-ViLG 模型](https://wenxin.baidu.com/wenxin/modelbasedetail/ernie_vilg/) 虽然有着不俗的实力（虽然训练数据集更小），但是依然生成不了带有天安门的图片（[详见](https://www.technologyreview.com/2022/09/14/1059481/baidu-chinese-image-ai-tiananmen/)）。

→ [介绍原文](https://mp.weixin.qq.com/s/_XJPrxQFo6a7apPPMKDDiw)

---

# 重读HIG（说明）

本节本应是重读 Human Interface Guidelines 系列连载第十一期。但为避免本期（以及之后）篇幅过长，便暂停一期发布，但新旧内容都已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上，有兴趣可以先去阅读。

---

# 摘录

这周看过的一些——

> Our goal is to be Figma not Adobe

—— Dylan Field - [出自](https://twitter.com/zoink/status/1355173534390075394)

---

# 小事

1、Adobe 以约 200 亿美元现金和股票和 Figma 达成协议，共用迎接未来协同创作的时代。

这一消息震惊了很多设计师，Adobe 囊中掏出了 Figma 50 倍ARR，其当天股价也趁势大涨 -16% 之多，走在 SNS 的大街上都能看到 meme 纸片漫天飞舞，仿佛 Dynamic Island 不曾发布过一样。

→ [交易新闻稿](https://news.adobe.com/news/news-details/2022/Adobe-to-Acquire-Figma/default.aspx)

Adobe 是谁——开发了 Illustrator，曾经桌面排版的定义者，有着 Adobe Original 字体库，[软件大买家](https://en.wikipedia.org/wiki/Adobe_Inc.#Anti-competitive_practices)，因 Adobe Flash 的安全性能、定价不公平和无视贫穷的个体创意工作者而臭名昭著，是 Microsoft 的合作伙伴；

Figma 是谁——高性能 Web 技术拥护者，全世界设计师的工作大脑支配者，设计社区文化的传播者，PLG 模范学生，协同工作提高了设计师话语权，并会偷偷从你的信用卡划出多个 15 美元账单，是 Microsoft 的合作伙伴；

> 「我们上周失去了女王，这周又失去了 Figma。」—— 某英国设计人员

![截屏2022-09-16 13.47.40.png](Scenes%20Weekly%20%2370.assets/%E6%88%AA%E5%B1%8F2022-09-16%2013.47.40.png)

{上图：截自 Figma vs Adobe XD 的页面}

[Dylan Field](https://twitter.com/zoink) 说你先别急，我们 Figma 会从 Adobe 那里师夷长技（包括图像处理、视频、插画、3D 和字体），哦听起来真不错，虽然不指望用上滤镜库、表达式和 Adobe Fonts，但是能加强现在的字体选择预览和一些 3D 支持就更好了。可以的话，希望把 Adobe Max 的技术也拿过来用用，顺便验证下是否真的存在。当然比作 Apple 收购 NeXT 还是有点高期待了。

Field 又说，Figma 将会保持自主运营。他不光自己说，还在[对媒体说](https://www.protocol.com/workplace/adobe-figma-dylan-field-user-reactions)，还对[手下员工](https://twitter.com/rogie/status/1570558838885208064)说，告诉你们设计圈的父老乡亲们，Figma 不会推出 30 天试用然后付费后不让你取消订阅的模式，你们不必把 Figma 拖到 Adobe Zii 2022 的窗口中。不光 Field 说，之前被收购的 Frame.io 的设计 VP [也在说](https://twitter.com/kurtvarner/status/1570563580055130115)，我们 Frame.io 活的好好的，Adobe 一直很尊重我们的决策。哦，挺好。

Adobe 说什么了，没说什么，总之先安抚股东。反正说什么都会被骂。

Sketch 说，嘿伙计，还记得懵懂年纪时，在苹果湖畔上我们的初次邂逅吗？森林不会忘记，世界也不会忘记，我们也是。那份做 logo 和崩溃丢失设计稿的回忆永远在我心中，💎钻石恒久远！

![截屏2022-09-17 21.32.16.png](Scenes%20Weekly%20%2370.assets/%E6%88%AA%E5%B1%8F2022-09-17%2021.32.16.png)

{上图：Sketch 目前在其官方 Twitter 置顶的视频截图}

这话听了 Apple 都流泪，但如果被 Microsoft 看到了应该会说省省吧，眼泪不值钱。事实上，在这个事件中， Microsoft 一直都很沉默。我在[第 68 期](https://designscenes.zhubai.love/posts/2178446713948692480#:~:text=5%E3%80%81-,Microsoft,-%E5%92%8C%20Adobe%20%E7%9A%84)介绍了 Microsoft 与Figma、Adobe 的不菲关系。不难看出，Adobe 收了 Figma 后，Microsoft 不管取不取消 CC 订阅咱还是一家人。

FTC 呢，FTC 说话 FTC。FTC 一如既往地沉默并扔出一个[链接](https://www.ftc.gov/advice-guidance/competition-guidance/guide-antitrust-laws/mergers/competitive-effects)，在 Adobe 的暴君行动前，估计找不到什么证据。设计领域划分很复杂。

Figma 的社区成员只能做做 [meme](https://prototypr.io/post/adobe-figma-meme) 发泄一下，一起[为 Figma 上香](https://www.figma.com/file/4mnaXLNqGVUPGnxIB8msRF/%F0%9F%96%A4-RIP-Figma-%F0%9F%96%A4?node-id=97019:10294)，哈哈了事后继续打工。这可不像 [ADOBE SUCKS](https://ass.easun.me/) 那样找替代，比如看看[这篇文章](https://stackdiary.com/figma-alternatives/)推荐的 5 个 Figma 替代，除了 Sketch 都不咋行。倒是观察者网可以举例国产即时设计、MasterGo（虽然我拼写对了但我不是水军）、Pixso 和*摹客等后起之秀。*

明天太阳照常升起。

---

2、如今各个图像生成模型所使用的训练数据集基本是灰色地带，Have I Been Trained? 这个网站便可以按文字或图像搜索，查验一张图是否在 58 亿数据集中被用于 AI 训练。

![截屏2022-09-17 23.13.30.png](Scenes%20Weekly%20%2370.assets/%E6%88%AA%E5%B1%8F2022-09-17%2023.13.30.png)

{上图：搜索狗出现的结果}

如上图搜索狗出现的结果，可以看到很多张付费图库的预览图，带着水印。

→ [网站](https://haveibeentrained.com/)

---

3、很多播客背后的赞助都是 VPN 厂商，Michael Girdley 找到一份小型 VPN 公司 2020 年的损益表，背后的暴利不言而喻。

![1b5fd5f6-d0be-46c0-ba31-7493878f6fcf_2870x1022.png](Scenes%20Weekly%20%2370.assets/1b5fd5f6-d0be-46c0-ba31-7493878f6fcf_2870x1022.png)

{上图：Here is a small-scale VPN business’ P&L statement from 2020.}

可以看到净利比重相当高，现金充足。而 VPN 这行的特点是，商品差异性低，因为所使用的软件很多都是开源的。顾客终身价值低，获客成本高，VPN 厂商入局的又多，导致大家都在通过各个渠道挤出新客户，亦或者是直接并购其他对手。

→ [原文](https://girdley.substack.com/p/why-is-every-podcast-sponsored-by)

---

4、还记得几年前一款新奇的聊天应用 Die With Me 吗？只有在你的手机电量小于 5% 时才可以进聊天室交流。他是艺术家 Dries Depoorter 和开发商 David Surprenant 合作的实验产品。如今 Depoorter 又有一个新的有趣项目 The Follower。

![截屏2022-09-17 23.36.57.png](Scenes%20Weekly%20%2370.assets/%E6%88%AA%E5%B1%8F2022-09-17%2023.36.57.png)

{上图：左图是路人的 Instagram 照片，右图是公共摄像头捕捉到了路人拍照过程}

The Follower 项目的目的是监视一个公共摄像头一段时间，找出摄像头所在位置的所有 Instagram 照片，通过软件（机器识别）找出这些照片的拍摄过程。为期 10 天，在 22 号公布结果。

→ [围观](https://driesdepoorter.be/thefollower/)

---

5.1、又一篇直观的二维码介绍文章，由 Twitter Threads 整理而成。

→ [原文](https://typefully.com/DanHollick/qr-codes-T7tLlNi)

5.2、在[第55期](https://designscenes.zhubai.love/posts/2140365736035151872#:~:text=%E4%BD%BF%E7%94%A8%E7%9A%84%E6%98%AF%E4%B8%80%E9%A1%B9-,Smart%20Brevity,-%C2%AE%20%E7%9A%84%E6%8A%80%E6%9C%AF%EF%BC%8C%E9%9B%86%E6%88%90)提到新闻媒体 Axios 所使用的 Smart Brevity® 写作风格，Axios 后来出版了一本书 *[Smart Brevity: The Power of Saying More with Less](https://bookshop.org/p/books/smart-brevity-the-power-of-saying-more-with-less-roy-schwartz/17897762?ean=9781523516971)* 遭到 TNR 的批评：这本书的写作，既不简洁也不智能。

→ [批评](https://newrepublic.com/article/167733/axios-guide-writing-well-neither-smart-brief-smart-brevity-book-review)

5.3、2022 年搞笑诺贝尔奖

→ [乐](https://cen.acs.org/people/awards/2022-Ig-Nobel-Prizes/100/i33)

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

![WOLONG.png](Scenes%20Weekly%20%2370.assets/WOLONG.png)

{上图：卧龙 苍天陨落}

这周体验了 VALKYRIE ELYSIUM 和 WOLONG 在 PS5 上的 demo。前者的战斗手感没有预想的那么差，起码比第一次接触星之海洋系列时更好上手。虽然解放了单维度战斗方式，但保留了和英灵协同作战的设定。迷宫方面失去了传统多维度平台解密的特色，不知正式版会有何惊喜。

卧龙则在满是仁王味道的瓶子中装上了新酒，但是敌人出击更快，化劲的（弹反）失败和成功都反馈巨大，双向的气槽设定让攻击与防守紧密相连，使得战斗比仁王还要紧凑。由于化劲和翻滚绑定同一按键（区别是按一次和按两次），所以对以往无脑翻滚的惩罚也更加苛刻。作为 Team NINJA 的又一诛死类游戏，万众期待。

→ [VALKYRIE ELYSIUM](https://store.steampowered.com/app/1963210/VALKYRIE_ELYSIUM/)

→ [卧龙：苍天陨落](https://store.steampowered.com/app/1448440/Wo_Long_Fallen_Dynasty/)

---

# 映像

现实拟像放映——

![4000.png](Scenes%20Weekly%20%2370.assets/4000.png)

{上图：奥克兰画廊天花板上的酸黄瓜}

这枚被扔到天花板的麦当劳汉堡中的配料 pickle， 标价 10,000 新西兰元（约人民币  41,849 元）。

> “It’s not about the virtuosity of the artist standing there in the gallery throwing it to the ceiling – how it gets there doesn’t matter, as long as someone takes it out of the burger and flicks it on to the ceiling,” Moore said.

> “The gesture is so pure, so joyful … that is what makes it so good.”

---

# 温故

→ [Scenes Weekly #21](https://mp.weixin.qq.com/s/G0oOMg331FbhQxDUq01SLg)

- Telegram 8.0 贴纸回执
- 赫尔辛基文化中心 Kaapelitehdas 的动态标识
- Processing 的21周年新标识
- Commercial Type 公开草案字体
- NFT 马桶碎片
- 隐私友好型统计工具 Plausible
- Epic 和 Apple 诉讼战中公布的100多件细节
- 设计师社区的构建难题
- 自动驾驶伦理困境
- 古代欧洲地区纹章查询

---

喜欢本文的话，欢迎分享、订阅。

第 69 期请[在此查看](./Scenes Weekly #69.md)。

本次封面使用了 Adobe Clean 字体。