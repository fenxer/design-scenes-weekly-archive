# Scenes Weekly #74

2022-10-24

\> 设计视角下的世界——

第 73 期请[在此查看](./Scenes Weekly #73.md)。

本期出现：

- Figma 删除锚点细节
- 重读HIG（十四）
- 维基基金会的财务状况
- iPhone 激光雷达扫描试玩
- 低迷的 Patreon
- GitHub Copilot 审查
- 其他：文案集合 Copy Book、BeReal 如何启动、RTX 4090、AT Protocol、网页中使用 Display-P3、详解声音、Photoshop for Text、DuckDuckGo for Mac beta 公测、奥利奥联动、图片生成 prompts

如有格式异常建议点击最上方「在浏览器中访问」。

---

封面图由 Adobe Express 制作，顺便拿 Apple ID 新注册了一个外区的 Adobe 账号。原本是想体验 [Advanced AI](https://twitter.com/jnack/status/1582818166698217472) 加持下的字型生成功能，不过发现还没上线。我没用过 Canva 所以说不出一二。

另外也更新了一下 Figma 上的[封面归档](https://www.figma.com/community/file/1139404827019734932)，之前一直忘记发布到社区……

最后欢迎上周的新订阅者，感谢所有订阅者的支持🫣

---

# 没事

1、 在 Figma 中直接删除矢量图形的一个锚点，所处路径也会随之删除。可是选择该锚点后按下 Shift + Delete，其所处路径便不会消失，而且根据删除锚点和两端锚点平滑该路径。

![b38f3b8b0b31acf9c51b5fde32275264d2020ca6-2120x1000.png](Scenes%20Weekly%20%2374.assets/b38f3b8b0b31acf9c51b5fde32275264d2020ca6-2120x1000.png)

{上图：使用 Shift + Delete 删除一段曲线中的锚点}

我上周才从 [Noah Levin 那里](https://twitter.com/nlevin/status/1582871788668694528)知道这个小贴士，但一查发现这是 2016 年的博客文章。那个时候我刚刚因为使用 Figma 卡顿而弃用回到 Sketch……最神奇的是，有时候两边端点没有手柄参数，Figma 也会做原曲线形状的拟合：

![heal.png](Scenes%20Weekly%20%2374.assets/heal.png)

{上图：在一条线段中间添加锚点，垂直拉动手柄形成曲线，然后按 Shift + Delete 删除}

 → [原文更多细节](https://www.figma.com/blog/delete-and-heal-for-vector-networks/)

---

# 重读HIG（十四）

本节是重读 Human Interface Guidelines 系列连载第十四期，目的为温故知新和跟进新内容。 为避免篇幅过长，不会一次发布太多，之前内容已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上。

### 管理账户（Managing accounts）

> If you require an account, consider using [Sign in with Apple](https://developer.apple.com/design/human-interface-guidelines/technologies/sign-in-with-apple/introduction) to give people a consistent sign-in experience …

谢邀，HIG 的这个建议你应当谨慎考虑，特别是当你的产品需要客服支持时。

> 💡拓展：[Why AnyList Won’t Be Supporting Sign In with Apple](https://blog.anylist.com/2020/06/sign-in-with-apple/?continueFlag=c1068e7e0e455bd9923ad0f16a65f620)

> AnyList 解释了他们的 app 为什么不使用 Sign in with Apple：虽然 Apple 的出发点是善意的~~（看你怎么想）~~，但除了第三方登录常见弊端外，隐藏电子邮件功能大大提高了客服成本，安全机制与跨平台性不太成熟，与 app 本身的邮箱分享功能不合等等角度，都影响了 app 运转。

- 向用户解释为何需要注册，能为用户带来什么好处；
- 尽可能滞后登录流程，先体验；
- 如果你没有使用 `Sign in with Apple` **，**HIG 建议使用 Passkeys 利用系统的生物识别来省去输入密码的步骤（为什么这时候不强调多平台注意事项了）。如果执意使用密码输入，则建议使用 [Password AutoFill](https://developer.apple.com/documentation/security/password_autofill/) 自动生成密码。
    - Apple 仿佛在告诉你，「来了就别想走了」。鉴于 HIG 是以 Human 开头，Apple 格局小了。
- 通常情况下，不要在应用内建一套专用的生物识别；
    - 我更在意「不通常情况」下是……
- 不要乱使用 **passcode** 这个词，容易被误认为机器解锁密码。在中文，Passcode 被翻译成密码已经混在一起，但多语言本地化时还是要注意一下；

后面是关于删除账户的注意事项，暂时没什么可说的。关于密码、登录与身份验证的问题，HIG 还有很多没谈，比如手机号登录、临时账户、默认登录身份等问题。而且一直在推销自己，避而不谈其他注意事项，👎。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/managing-accounts)

### 管理通知（Managing notifications）

通知这一节 HIG 最先提到的是专注模式（Focus）下的场景。建议开发者先为应用或游戏的通知定义一个分级。

首先时类似电话、短信的即时交流通知，称为 communication notifications。除此以外的其他通知都是 noncommunication notifications，有四个分级，重要程度从上到下依次提升：

- Passive：一些不太重要的信息，用户闲暇时可查看；
- Active：默认分级。一些用户想要知道的信息通知；
- Time Sensitive：对用户产生直接影响，需要立即了解的信息，比如账户安全问题。此时该分级的通知可打破专注模式规则；
- Critical：最重要的通知级别。频率极为罕见，一般涉及到来自政府或组织机构的健康、安全信息。此级别通知在静音模式下也可以通知；

不要将通知变成打扰，通知需要和用户建立信任。除非用户明确同意收到营销类通知，否则不要发送。而且也不要使用 Time Sensitive 和更改级别通知发送。最后在 app 中应有管理通知的设置。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/managing-notifications)

---

# 摘录

这周看过的一些——

> Keeping your UI as thin and transparent as possible is essential to clearly communicate your value, while offering the least amount of friction possible to get your customer to their desired outcome. Customers don't care about your product, they care about what they get from it.

—— [@traf](https://twitter.com/traf/status/1560275683577712640)

---

# 小事

2、维基百科（Wikipedia）大多情况下运行良好，但有时也会暴露出问题，比如今年发生的以卡申银矿为导火索的[伪历史事件](https://zh.wikipedia.org/wiki/Wikipedia:2022%E5%B9%B4%E6%AD%B7%E5%8F%B2%E7%9B%B8%E9%97%9C%E6%A2%9D%E7%9B%AE%E5%81%BD%E9%80%A0%E4%BA%8B%E4%BB%B6)，又诸如[第63期](https://designscenes.zhubai.love/posts/2165749375996317696#:~:text=%E7%9A%84%E4%BB%96%E5%9C%A8%E4%B8%8A%E5%91%A8-,Wikipedia,-%E9%A1%B5%E9%9D%A2%E7%AA%81%E7%84%B6)介绍过的编辑反馈和司法影响问题。不过这次要谈的是一个老问题——你向 Wikipedia 捐款过吗？

如果没有的话，不，不必捐了。

很多捐款文案会营销成，如果没有你的捐款，我们的项目就要倒闭或无法独立运营下去，但维基基金会（Wikimedia Foundation, WMF）可不是这样。在 [WMF 2020-2021 全年财务报表](https://upload.wikimedia.org/wikipedia/foundation/1/1e/Wikimedia_Foundation_FY2020-2021_Audit_Report.pdf)（目前最新审计）中我们能看到 WMF 2021 年：

- 总流动资产是 208,678,345 美元
- 来自捐赠的金额为 153,096,642 美元
    - 赠手续费就有 6,386,483 美元
- 人力支出 67,857,676 美元
    - WMF 有 450 多名员工。虽然有很多技术和运营人士，但筹集资金这方面 WMF 有几个[专门的部门](https://wikimediafoundation.org/role/staff-contractors/#advancement)负责，很多专家，多达 46 人……甚至还有一位[横幅专家](https://wikimediafoundation.org/profile/haley-nordeen/)（Banner Specialist）😅
- 服务器支出仅 2,384,439 美元
- 到 2021 年末净资产结算为 231,177,536 美元，对比同期 2021 年净资产是 180,315,725 美元
- 维基百科条目志愿者编辑和维护者支出：0 元

>  The bureaucracy is expanding to meet the needs of the expanding bureaucracy.

UnHerd 的报道常常带有一定的偏颇，但在[报道这种文章](https://unherd.com/thepost/the-next-time-wikipedia-asks-for-a-donation-ignore-it/)时却显得有些适合。  对 WMF 的[口诛笔伐](https://www.theregister.com/2012/12/20/cash_rich_wikipedia_chugging/)也不仅是今年才有，支出不透明、技术迭代缓慢以及大量用于维基百科之外的活动资金都是 WMF 的「[癌症](https://en.wikipedia.org/wiki/User:Guy_Macon/Wikipedia_has_Cancer)」。比如 2021-2022 年度计划中，拨款3670万美元的「蓬勃发展的维基媒体运动」**具体**在做什么一直含糊不清。

![截屏2022-10-20 14.28.20.png](Scenes%20Weekly%20%2374.assets/%E6%88%AA%E5%B1%8F2022-10-20%2014.28.20.png)

{上图：WMF 年度计划中，蓬勃发展的维基媒体运动的重点领域}

下次捐款或许该考虑更多其他项目，比如 [Internet Archive](https://archive.org/)、[Aeon](https://aeon.co/) 或者 The Marginalian 这样的 newsletter [1]，或者直接忽略掉。

[1]：不构成捐赠建议。

---

3、iwama 科普了 iPhone 上 3D 扫描 app 的一些背景和对比。

首先要了解的是，iPhone 的 3D 扫描依赖于手机内置的激光雷达（LiDAR）感应器。

- iPhone 激光雷达照射距离为 5 米，小于工业激光雷达仪器，可能是电源消耗限制；
- 由于需要移动扫描，精度也较低；
- 激光照射密度低，像是平面上细电线可能扫描不到；
- 市面上 3D 扫描大概分两种方式，Mesh 式（按面创建）或点云式（按3D坐标点创建），一些应用还会结合原本的摄像头采集纹理；

iwama 推荐了三个应用作为 3D 扫描的入门体验：

- [Scaniverse](https://apps.apple.com/cn/app/scaniverse-3d-scanner/id1541433223)。免费。媲美收费应用级别的扫描效果，被 Niantic 收购后变为免费软件。特点是自动平滑网格，可本地渲染。
- [WIDAR](https://apps.apple.com/cn/app/widar-3d-scan-edit/id1574012258)：免费。唯一一款支持 Android 平台的 3D 扫描应用，可使用照片合成扫描。特点是可置入其他用户扫描的模型。
- [Trnio](https://apps.apple.com/us/app/trnio/id683053382)，4.99美元，不支持国区 App Store。纯摄影合成扫描，在云端处理扫描结果，适合拍摄扫描户外物体。

![1654527231659-4FjgstTaZ9.jpeg](Scenes%20Weekly%20%2374.assets/1654527231659-4FjgstTaZ9.jpeg)

{上图：iwama 制作，更详细版的应用对比}

扫描时应该注意：

- 激光会穿过透明和半透明物体，无法拍摄；
- 一些带有高反射率的光滑表面会因不同角度反射信息不同，而被识别成其他物体。可以适当遮挡住一些入射光线，但整体环境不能太暗（户外阴天你懂的）；
- 线、纸等一些细或薄的物体会因精度问题无法识别；
- 表面单色或者是规则图案的物体会影响 VIO 定位而影响扫描效果，可以随意贴一些和纸胶带或其他东西打乱图案；
- 一些表面特别复杂的物体，有时会因面数太多合并；
- 动态物体无法扫描；
- 不要离扫描物体太近，理想距离是 0.5m~3.0m 左右；
- 扫描地面时，要有一定角度而不是垂直地面扫描，大概 30° 左右；
- 如果是拍摄多张照片的方式合成 3D 模型，保证每张照片之间有70% 的重合覆盖效果比较好，但也要注意拍摄照片上限；
- 提前规划好摄影扫描路径，别摔到自己；

![1655806650926-oLIXzEl6q4 大.jpeg](Scenes%20Weekly%20%2374.assets/1655806650926-oLIXzEl6q4%20%E5%A4%A7.jpeg)

{上图：摄影合成扫描时，拍摄照片角度分布建议}

我也使用 Scaniverse 试了一下，高精度渲染效果惊人，比之前使用前摄像头合成好很多。但是稍微小一点的东西便难以识别。

![Scaniverse.png](Scenes%20Weekly%20%2374.assets/Scaniverse.png)

{上图：使用Scaniverse 扫描家中一个体素拼装玩具}

虽然目前激光雷达大多应用在摄影辅助或生物识别上，但原文最后的应用举例还是出乎我的预期——东京都政府的数字服务发展部门（デジタルサービス推進部）鼓励民众使用智能手机上的激光雷达功能，帮助上传和构建一些城市元素的点云数据和模型，这里是[测试报告](https://info.tokyo-digitaltwin.metro.tokyo.lg.jp/zissyou03/)。工业激光雷达扫描诚然质量更好但是成本更高，跟不上日益变化的城市，可能今天这里放着一个自动贩卖机，第二天就被挪走了，简单地使用智能手机更新城市数据可能更加便捷。

![截屏2022-10-20 16.23.20.png](Scenes%20Weekly%20%2374.assets/%E6%88%AA%E5%B1%8F2022-10-20%2016.23.20.png)

{上图：使用手机激光雷达更新补充地图元素}

→ [原文](https://note.com/iwamah1/n/n48a549845ae3)

---

4、我有很长时间没关注 Patreon ，直到最近听说该公司裁员 17%（80人）以及其他业务裁减调整。这是 9 月 13 号的[公告](https://blog.patreon.com/a-note-from-jack)内容，在此前十天，根据泄露的财务VP Carlos Cabrera内部备忘录，随着 COVID-19 恢复，Patreon 409A 估值过去一年下降了 70% 之多（39.45 → 12.10），这既有宏观经济环境影响，也有公司自身的问题。

Patreon 的模式一直比较重商务资源而轻模式。除了收购 Memberful 之外听不到「科技的声音」。看 Insider 报道，Patreon 重金邀请过来的创作者/TikTokers Larray 和 Lil Huddy 并未达成预期效果（Z世代教训），比这两场百万美元交易更大的是他们还找过 MrBeast，当然谈判也未达成。看不清市场的 Patreon 即便在一季度手握 2.49 亿美元现金和1.2 亿美元订阅收入，但是依然决定裁员（裁员待遇还不错）。

至于 Patreon 自身，在混乱的审查制度和糟心的用户体验之外，Patreon 对于自身平台的定位也摇摆不定，多年来 Patreon 从未成功建立属于自己的内容平台，对于大部分创作者依然遵从引流到 Patreon 的旧模式，随着其他源内容平台建立起自己的内容变现渠道，Patreon 的弱点逐渐暴露出来：分发能力孱弱，创作者之间几乎都是「孤岛」，给创作者的数据分析形同虚设，移动应用简陋等等。这些恰好是创作者们所渴求的，如下图。

![Future-Aspirations.png](Scenes%20Weekly%20%2374.assets/Future-Aspirations.png)

{上图：Patreon 2022年官方推出的创作者调查报告显示，创作者最想要的是增加受众}

久违地登录了 Patreon，查看了一些关注的创作者们，谢天谢地他们的收入看起来依然不错，希望没有被平台影响太多。

↓ 参考

[Leaked memo reveals Patreon's valuation plunged 70% in the past year and the company is postponing its IPO plans](https://www.businessinsider.com/patreon-valuation-plunged-past-year-ipo-postponed-leaked-memo-2022-10)

[Patreon's deals with top TikTokers fell far short of expectations, leaked documents show](https://www.businessinsider.com/patreon-layoffs-company-documents-insiders-reveal-creator-partnership-struggles-2022-9)

[Why Patreon is struggling](https://simonowens.substack.com/p/why-patreon-is-struggling)

---

5、Matthew Butterick 有着作家、设计师、程序员和律师的身份，看起来是审查 GitHub Copilot 的优秀人选——事实上也这么做了。今年 6 月份他就开始[痛斥 Copilot](https://matthewbutterick.com/chron/this-copilot-is-stupid-and-wants-to-kill-me.html)，现在他重新拾起[律师资格](https://apps.calbar.ca.gov/attorney/Licensee/Detail/250953)，准备收集材料试图起诉 GitHub Copilot 所使用的代码侵犯了开源社区权利。

→ [GitHub Copi­lot inves­ti­ga­tion](https://githubcopilotinvestigation.com/#)

这可能涉及到两方面：

- Copilot 所使用的训练数据是否可被合规地使用？
- Copilot 所生成的代码结果是归于借鉴还是抄袭？

就平时逻辑来说，作为人类自身我们也会通过其他人作品来学习，并化为自己的知识展现出来，比如本通讯。当主体是机器学习时，事情变得更加复杂，Butterick 也在广泛征集和取证，无论成功与否，都能代表当今司法对 AI 的态度。

---

6.1、[Copy book](https://copybook.me/) 是界面设计中一些英文文案集合网站，特色可以是用语气分类。

6.2、[First 1000](https://read.first1000.co/p/bereal) 梳理了 BeReal 应用白手起家的历史。

6.3、RTX 4090 在 [HashCat 基准测试](https://www.tomshardware.com/news/eight-rtx-4090s-can-break-passwords-in-under-an-hour)中两倍于 RTX 3090 性能，8 台 4090 可在48 分钟内尝试超过 2000 亿种组合。

6.4、沉默已久的 bluesky 项目推出 [AT Protocol](https://atproto.com/guides/overview) 社交协议。

6.5、网页 Display-P3 色域显示作为 Safari [独占功能](https://caniuse.com/css-color-function)已久，Chrome 108 开启相关 flag 后也将支持，该提前[了解一下](https://www.bram.us/2022/10/13/upgrading-colors-to-hd-on-the-web/)了。

6.6、传奇作者 [Bartosz Ciechanowski](https://ciechanow.ski/sound/) 又发布了新文章，这次讲的是声音。

6.7、Stephan Ango 在想象[文字版的 Photoshop](https://stephanango.com/photoshop-for-text)，一种可以给文字随意加「滤镜」的 AI 工具，新闻风、论文风、文学风那种。

6.8、DuckDuckGo for Mac beta [公测](https://spreadprivacy.com/duckduckgo-for-mac-open-beta/)，基于高度定制化的 webkit。

6.9、奥利奥想在你一周最忙的时候——特别是下午的黄金开会时间段——观看他的主题视频，并享用新的 Thins 系列饼干。还有大眼曲别针 Clippy [出镜](https://thedieline.com/blog/2022/10/18/microsofts-clippy-and-oreo-thins-team-up-to-give-you-a-well-deserved-snack-break?)。

![AnimatedImage.gif](Scenes%20Weekly%20%2374.assets/AnimatedImage.gif)

{上图：奥利奥与微软新的 emoji 联动表情图}

6.10、AI 做图的「产业链路化」已经过渡到 prompt 阶段，现在你可以使用 [img2prompt](https://replicate.com/methexis-inc/img2prompt) 或 [latentspace.dev](https://www.latentspace.dev/) 直接上传图片生成 prompt。

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

![GOLDEN.png](Scenes%20Weekly%20%2374.assets/GOLDEN.png)

{上图：The Case of the Golden Idol}

在事件现场，时间仿佛静止，你可以翻动在场人士的口袋，淘出所有信息，然后做出事件来龙去脉的「完形填空」，每一幕连在一起是一幅荒谬诙谐的反乌托邦闹剧。这款新型侦探游戏类似 Trick x Logic 但是更为简单一些，如果你也喜欢 [Return of the Obra Dinn](https://store.steampowered.com/app/653530/Return_of_the_Obra_Dinn/)，不要错过这款游戏。

→ [游戏获取](https://store.steampowered.com/app/1677770/The_Case_of_the_Golden_Idol/)

---

# 映像

现实拟像放映——

![7616 大.png](Scenes%20Weekly%20%2374.assets/7616%20%E5%A4%A7.png)

{上图：Sandbagged statue of Dante Alighieri in Volodymyrska Hirka Park}

基辅市圣弗拉基米尔山公园内的[沙袋雕塑](https://www.theguardian.com/world/2022/oct/18/sandbag-sculpture-kyiv-shielding-statues-from-russian-bombs?CMP=artweekly_email)

Photograph: Ed Ram/The Guardian

---

# 温故

→ [Scenes Weekly #25](https://www.craft.do/s/YNdfyUwCkh91p2/b/E19AD1E2-756A-47D0-9C85-5AB5FD28BE8D/Scenes_Weekly__25)

- Grilli Type 的新字体 GT Ultra
- Moe Amaya 的个性个人网站
- 平面设计相关收藏网站 Reading Deisgn
- Apple Fitness+ 优劣点
- AI 驱动的创意工具 VIZCOM
- Exposure 新标识
- Okhsv 和 Okhsl 颜色模型介绍
- Graphic Design History Resources
- OpenMoji
-  iPod 室外广告

---

喜欢本文的话，欢迎分享、订阅。

第 73 期请[在此查看](./Scenes Weekly #73.md)。

本次封面使用了 Adobe Express 中的 Abril Fatface 字体。

