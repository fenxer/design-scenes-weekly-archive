# Scenes Weekly #35

2021-12-20

\> 设计视角下的世界——

第 34 期请[在此查看](./Scenes Weekly #34.md)。

本期出现：Figma、WCAG 3.0、iOS 15.2、Blinkist A/B Test、TDesign、Airpods、Juniper、2021 State of CSS、Notion、Readymag Pojects of the Year、Grilli Kiosk、PNG Parser Differential、Wombo

如有格式异常建议点击最上方「在浏览器中访问」。

---

# 微博

1、从招聘移动端岗位人员，到测试和正式上线，Figma 的移动端应用改版历经了不少时间。新的应用除了保留 Mirror 功能外，还可以在手机上查看设计文件。

![8d11266f4d814ce48735dd00c10b945d.png](Scenes%20Weekly%20%2335.assets/8d11266f4d814ce48735dd00c10b945d.png)

{上图：Figma 移动端 App 截图}

上图右图中查看文件的界面，A 功能其实是切换 pages，但就我而言，这个图标太像复制功能了……结果也这么继承到正式版了。

→ 说明文档

[Guide to the Figma mobile app](https://help.figma.com/hc/en-us/articles/1500007537281)

---

2、仍处于草案阶段的 WCAG 3.0 已经受到越来越广泛的关注。内容上对之前 2.X 内容进行了囊括和扩展，但是语言更易懂，不以技术为导向，回归用户需求。还更新了包括对比度在内的各种测试机制。

如果说 WCAG 2.X 是一部「白皮书」，WCAG 3.0 更倾向于执行层面。它更注重实际结果产出以及如何达到所要的结果，怎么去做实事上的优化。

同时 WCAG 3.0 加入了总体评分，分为金、银、铜三个级别。在之前讲述工信部适老化的那条微博中也提到了类似评分标准。目前 WCAG 3.0 的评分还处于审核商榷时期。明年 WCAG 2.2 发布，所以 3.0 可能是个更漫长的过程。

![c98d381882f445c3adf2422e1351c6d1.jpeg](Scenes%20Weekly%20%2335.assets/c98d381882f445c3adf2422e1351c6d1.jpeg)

{上图：WCAG 3.0 网页头部截图}

WCAG 3.0 中引用的对比度的评级机制 APCA 比之前较大的变化，不向后兼容。

当前 WCAG 2.X 中一些需要改进的点为：2.X 将反转颜色视为相同对比模式（即白纸黑字等于黑纸白字），并且没有考虑字体的字重、字号以及字型本身与周围环境的搭配。

3.0 里目前有一套已经非常严苛的测试，这里简单摘录几点：

- 单位以 px 为标准； - 色彩空间以 sRGB 为标准； - 字号越小，字重越轻，越需要更大的对比度（很符合直觉）； - 建议 css 里的 font-smooth 设置为 auto。手动设置为 antialiased 会降低对比度。 - 行间距、字间距、行长、字体透明度、阴影等实际都会影响对比度和可读性； - 如果是在视网膜屏上做的测试，也请注意普通屏幕上的效果； - 里面还要求了一套及其苛刻的测试工作空间参数，详见评论链接里的 Develop 选项卡底部； 实际评级结果最明显的是，原本几比几的参数变为更直观的百分制，比如之前正文最低对比 4.5:1 变为了 60 刚刚及格，75分以上才算对比度友好。

[登录 Twitter，关注Dan Hollick 🇿🇦](https://twitter.com/DanHollick/status/1468958644364402702)

[Myndex™ Perception Research](https://www.myndex.com/SAPC/)

[Visual Contrast of Text Subgroup - Silver](https://www.w3.org/WAI/GL/task-forces/silver/wiki/Visual_Contrast_of_Text_Subgroup)

[Visual contrast of text | How-To | WCAG 3 | Web Accessibility Initiative (WAI) | W3C](https://www.w3.org/WAI/GL/WCAG3/2021/how-tos/visual-contrast-of-text/)

[W3C Accessibility Guidelines (WCAG) 3.0](https://www.w3.org/TR/wcag-3.0/#visual-contrast-of-text)

---

3、iOS15.2 优化了摘要样式，变为大中小三种「不规则」排列，颇有 Android 12 的非对称美感。解锁后通知缩略图依然没有优化，比如支付宝依然是个大大的积分标识。

![5327f0daa4c94587a802b08b580b6eac.png](Scenes%20Weekly%20%2335.assets/5327f0daa4c94587a802b08b580b6eac.png)

{上图：iOS15.2 解锁界面截图}

展开后的摘要外面又套上了一层卡片，间距不等。左滑时，如果接触点过于靠近最右边依然会触发打开相机的手势。

---

4、Growth Design 这次没做 user journey，而是分享了一组 Blinkist 的 A/B Test 案例，如下图。

![12450d8a2d614a6fa1ea08a859767727.png](Scenes%20Weekly%20%2335.assets/12450d8a2d614a6fa1ea08a859767727.png)

{上图：Blinkist 的 A/B Test 案例}

- A 组是标准的付费转化界面，有着吸引你眼球的标题，明确的价格和底部清晰的 CTA 按钮。但是刻意淡化了左上退出图标，价格下方的小字充满了欺诈感，而且还是年度付费，很不友好。
- B 组则是完全站在用户立场，去告知用户试用期的流程，增加透明度。但是没有告知用户能得到什么。

B 的转化比 A 多了 23%，但依然有优化空间，所以有了 C 组。如下图，在试用期流程中小字提示试用后可立即获得什么。当然这个界面需要建立在用户知道 Blinkist 是干什么的前提。

![12fb720d00f549ba80f21cb5fe738baf.png](Scenes%20Weekly%20%2335.assets/12fb720d00f549ba80f21cb5fe738baf.png)

{上图：针对B方案优化后的C方案}

更巧妙的是这后面。用户参与试用后，就可以用试用日期提醒为理由引导用户去开启宝贵的推送通知位。这一招醉翁之意不在酒让用户开启推送提升至 74%，并减少了55%的投诉。如下图。

![70afaf986ba848d285f03b6b6b4afc8e.png](Scenes%20Weekly%20%2335.assets/70afaf986ba848d285f03b6b6b4afc8e.png)

{上图：试用通知提示}

→ 详见原文

[How Blinkist Increased Trial Conversions by 23% (Ethically)](https://growth.design/case-studies/trial-paywall-challenge)

---

5、本该在 12 月 23 日开源宣发前上线的 TDesign 文档网站，今天（17号）就走漏了风声。Github 上已是公开库，Figma 链接也被传到各个群聊里。毕竟腾讯 + Figma的公开组合还挺稀奇的，不知道是否和27日举办的腾讯设计周有关联。

![f854ef2b35d644deb79a0188478428b7.jpeg](Scenes%20Weekly%20%2335.assets/f854ef2b35d644deb79a0188478428b7.jpeg)

{上图：TDesign 设计系统封面}

文档本身实在是「平平无奇」，可能是还没完善和迭代。颜色模型只是单纯列出了16进制。产品特性说「支持使用者通过 Design Token 对设计风格进行扩展」，但是没有对 Token 的语法做设计性上的说明。整体排版貌似也没有优化。

近几年开源的力量逐渐渗入到设计领域，但不得不说大多数设计资产仍具有封闭性。越来越多的厂商愿意公开透明推动设计系统发展，这是大家都愿意看到的。

→ GitHub

[GitHub - Tencent/tdesign: Enterprise Design System](https://github.com/Tencent/tdesign)

---

# 摘录

> 假如您喜欢我的诗

> 又何必在意诗是我写的，他人写的，

> 或是无名氏写的呢？

> 其实，您读过的诗实际是自己的：

> 您就是作者，当您读诗的时候，您已经在作诗。

—— José Emilio Pacheco - Los trabajos del mar (1983) [翻译：梅娜](https://mp.weixin.qq.com/s?__biz=MzIyMTM0MzkxNA==&mid=2247483885&idx=1&sn=dd188eb593e83890b67ce18644c15ad0&scene=21#wechat_redirect)

---

# 杂事

1、Apple 在面向终端用户环节里，所擅长做的简化工作是有目共睹的，就像第一次使用 macOS 时那种便利。但当苹果的善意被施加在增加利润时就变得不是那个味道了。据传闻 Apple 推出了Airpods 固件升级工具，但是仅为技术人员提供。一般情况下 Airpods 会静默升级，但是要手动升级的话就要做一边充电一边重置等麻烦的事情。

→ 消息源

[登录 Twitter，关注Stella - Fudge](https://twitter.com/stellafudge/status/1469402228352032774?s=21)

---

2、Juniper 在澳洲为女性提供远程诊疗服务，其品牌由母公司 Eucalyptus 内部团队设计。

![130e67131788221.jpeg](Scenes%20Weekly%20%2335.assets/130e67131788221.jpeg)

{上图：Juniper 标识}

Juniper 整体采用了 Colophon Foundry 的 Nib 字体字型，然后把小写字母 i 上的点替换为叶子图形。这种设计灵感来自于对绿色植物的品质提炼——有韧性、有力量、坚强又脆弱。

![J-2.png](Scenes%20Weekly%20%2335.assets/J-2.png)

{上图：Nib 字体中一些细节}

我自己一直很喜欢楔形衬线字体所拥有的力量感和严肃感。但是 Nib 这款字体在一些地方做了圆润的处理，使得整体刚柔并济。对于 Juniper 这个品牌来说确实很合适。

→ 项目详情，你还能看到受马蒂斯影响的插画风格

[Juniper](https://www.behance.net/gallery/131788221/Juniper)

---

3、Sacha Greif（[sidebar.io](http://sidebar.io) 创始人） 联合一些开发者和团队，收集了8714份调研结果，发布了 2021 State of CSS。这里只看看 Typography 和 Accessibility 部分。

![截屏2021-12-16 16.28.16.png](Scenes%20Weekly%20%2335.assets/%E6%88%AA%E5%B1%8F2021-12-16%2016.28.16.png)

{上图：2021 State of CSS 主视觉，网页中有动画效果}

Typography 主要是可变字体、Opentype 特性和字体渲染相关技术。调查中，从未听过Opentype 特性相关属性 font-variant-* 的从 2019 年的 47.1% 到2021年的52.5%……实际用的人也越来越少。考虑到设计落地时也较少有可变字体的使用场景，所以可变字体在2022年的应用依然是个「新鲜」东西。而像 font-variant-numeric 这样的使用有七成人不知道，更让人深有隔行如隔山的感觉。font-display 和 line-clamp 这样偏开发解决方案的技术也没有更普及。

Accessibility 部分主要是 prefers-* 系列特性的应用，prefers-reduced-motion 和 prefers-color-scheme 的使用人数都有不小的增加，prefers-reduced-data 至今没有正式版浏览器支持所以96%的人没有听过和使用。color-contrast() 同样几乎没人使用，不知道是需求不多还是换用其他方式实现。tabindex 和 aria-* 特性在[第27期](https://mp.weixin.qq.com/s/7Zc01PKTDO5R_TB70w0MLQ) 腾讯兔小巢反馈社区的适老化与无障碍改造的文章中提到过，这两个特性都有九成的开发者听过和使用过！

调查的总结显示认为 CSS 易于学习的人数逐年减少，但是 enjoy writing CSS 的人却逐渐增加，祝大家都不会在繁杂的工作中失去那份热情与初衷。

→详细调查结果

[The State of CSS 2021](https://2021.stateofcss.com/en-US/)

---

4、Notion 起家的故事感觉很多人都听过了。看完感觉……日常羡慕国外有 Product Hunts、DN、HN 这种平台。

![https___bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com_public_images_175610f9-d6a6-40ba-8d6a-28c4a87a9f7f_1214x1256.png](Scenes%20Weekly%20%2335.assets/https___bucketeer-e05bbc84-baa3-437e-9518-adb32be77984.s3.amazonaws.com_public_images_175610f9-d6a6-40ba-8d6a-28c4a87a9f7f_1214x1256.png)

{上图：Notion 的对用户成本对价值比例的不断提高，通过口碑传播进一步扩大优势}

→ 如果没读过 Notion 的故事

[✨Notion](https://read.first1000.co/p/notion)

---

5、有着独特审美的建站平台 Readymag 今年推出了 Projects of the Year。共分为五类：Typography, Navigation, First page, Visual storytelling 和 Mobile。第一名可获得 $1500，第二名续费一年 Business plan，所有提名者都可以获得一份 Readymag 小礼品。

![截屏2021-12-17 17.28.12.png](Scenes%20Weekly%20%2335.assets/%E6%88%AA%E5%B1%8F2021-12-17%2017.28.12.png)

{上图： Readymag Projects of the Year 头图}

里面的网站称光怪陆奇，它们大都是从概念落地到设计的，非常适合扩展审美边界。顺便一提本通讯[第19期](./Scenes Weekly #19.md)曾介绍的 GRIDS 获得了 Storytelling 分组的第一名。如果对 Readymag 比较陌生，也可以看看我之前写的一篇介绍文章（[Notion](https://fenx.work/Showing-Readymag-2ef54e1b7322487e9435b360597661cb) / [公众号](https://mp.weixin.qq.com/s/hCtFPftq3Lu3BT40S2emBw)）。

→ 查看所有提名网站

[2021: Projects of the Year](https://readymag.com/readymag/projects-of-the-year-2021/)

---

6、Grilli Type 开了一个在线小店，卖一些制作某个字体时「一起做的奇怪的东西」。比如印有 Specimen 字样（即指字体样本的那个样本）的帽子，GT America 旗帜等等。

![daniel-faro_grilli-type_7S0A0419_lowres_650x@2x.jpeg](Scenes%20Weekly%20%2335.assets/daniel-faro_grilli-type_7S0A0419_lowres_650x@2x.jpeg)

{上图： 2019 GT Newspaper 商品}

→ 走过路过瞧一瞧看一看

[Grilli Kiosk](https://grillikiosk.com/)

---

7、趣闻：David Buchanan 在制作自己的多线程PNG解码器时遇到了一些数据块的独立解码 [bug](https://github.com/DavidBuchanan314/parallel-png-proposal/issues/3)，并将此漏洞应用到 Apple 自己创建的 PNG 数据块 iDOT 上，做出了能在苹果和非苹果浏览设备上的图片差异。如下图，Hello World 是在 Chrome 上打开的网页图片，Hello Apple 是在 Safari 上打开展示的图片。

![屏幕快照 2021-12-17 的 19.37.41 下午.png](Scenes%20Weekly%20%2335.assets/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202021-12-17%20%E7%9A%84%2019.37.41%20%E4%B8%8B%E5%8D%88.png)

{上图： Chrome 和 Safari 浏览器查看同一张图对比}

作者同时推出一个小工具来合成这样的图片。

→ 工具

[GitHub - DavidBuchanan314/ambiguous-png-packer: Craft PNG files that appear completely different in Apple software [NOW PATCHED]](https://github.com/DavidBuchanan314/ambiguous-png-packer)

→原文

[https://www.da.vidbuchanan.co.uk/widgets/pngdiff/](https://www.da.vidbuchanan.co.uk/widgets/pngdiff/)

---

8、Wombo 是一个根据文本就能生成不同风格图像的AI工具，共13种风格。

![屏幕快照 2021-12-18 的 14.34.09 下午.png](Scenes%20Weekly%20%2335.assets/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202021-12-18%20%E7%9A%84%2014.34.09%20%E4%B8%8B%E5%8D%88.png)

{上图：根据 Design Scenes 生成的图像}

生成的图像可以自己购买实体版，或者制作成NFT……

→ 也有移动端应用

[Dream by WOMBO](https://app.wombo.art/)

---

# 劳逸

![a4fd0febf5304050a08f991a61417900.png](Scenes%20Weekly%20%2335.assets/a4fd0febf5304050a08f991a61417900.png)

{上图：Heavenly Bodies Logo 与游戏里面操控的人物}

太空 QWOP ！

用双摇杆和四个键位控制宇航员在太空中完成一些任务。基于物理引擎，可双人co-op，流程不长，适合等待新游戏时打发时间。

→ 游戏获取（也支持 PlayStation）

[Steam 上的 Heavenly Bodies](https://store.steampowered.com/app/1138850/Heavenly_Bodies/)

---

# 映像

现实拟像放映——

图片加载中

![54c853fdf94a4376a9143681d8b736d1.jpeg](Scenes%20Weekly%20%2335.assets/54c853fdf94a4376a9143681d8b736d1.jpeg)

{上图：夕阳西降的70次曝光照片拼接}

> On August 20, 2018, these 70 exposures illustrate the descent of the sun, at 30 second intervals beginning at 07:21:48 pm Pacific Daylight Time, as it shines through the heavy wildfire smoke.

©David Ellingsen - Wildfire

注：Ellingsen 住在加拿大卑诗省，自 2017 年该地就有强烈的烟雾笼罩城市。上图就是 Ellingsen 记录的 2018 年一次烟雾中的日落景象。

---

喜欢本文的话，欢迎分享、订阅。

第 34 期请[在此查看](./Scenes Weekly #34.md)。

本次封面使用了 Ultra 字体。