# Scenes Weekly #45

2022-03-14

\> 设计视角下的世界——

第 44 期请[在此查看](./Scenes Weekly #44.md)。

本期出现：Huemint、Steam Deck、SingleFile、MDN Redesign、awwwards 2021、東京TDC賞2022、Inspecting in macOS、M1 Ultra、Windows Defender、Apple Music UX、Substack App、StyleNeRF、POCKIT 、GIF format

如有格式异常建议点击最上方「在浏览器中访问」。

---

# 微博

Huemint 使用机器学习去生成一套调色板，在每次生成的颜色中可以锁定想要的颜色，根据一定的对比度准则来生成随机色板。还可以调节 Creativity 来更变颜色采样的范围，如图。

![b9f866430e8c4860b3aaf1dd9eb246aa.png](Scenes%20Weekly%20%2345.assets/b9f866430e8c4860b3aaf1dd9eb246aa.png)

{上图：示意图片之一，红色和黑色都是可变换的}

生成后的色板会按照品牌设计、网站设计、渐变、插画等场景自动生成一些灵感向的示例。

→ 官网

[Huemint - AI color palette generator](https://huemint.com/)

---

# 摘录

这周看过的一些——

> And now the guidance of grace will be brought to the Tarnished who were spurned by the grace of gold and exiled from the Lands Between. Ye dead who yet live, your grace long lost, follow the path to the Lands Between beyond the foggy sea to stand before the Elden Ring. And become the Elden Lord.

—— Elden Ring - Prologue Text

---

# 杂事

1、想要颠覆主机业界规则的 Steam Deck 展示了其 512GB 版本独占的键盘主题 DEX-85。和国产输入法主题有得一拼。

![SD0K.png](Scenes%20Weekly%20%2345.assets/SD0K.png)

{上图：Steam Deck 中多种键盘主题展示}

前几天看 LTT 的 Steam Deck 软件评测感觉到，Valve 对 Steam 产品欠下的多年设计债终于得到了「回报」。访问速度慢、流畅性差、没有针对主机做一些主导航的肩键切换等等。一个很大的亮点是 Steam OS 自带了性能监测器，说明 Valve 首先足够了解产品面向的人群，加上最近相当频繁的更新，相信 Valve 会越走越远。

→ 评测视频

[【官方双语】Steam Deck是个不完全体 - Steam Deck软件评测#linus谈科技_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1744y1K74d)

---

2、SingleFile 这个浏览器插件可以保存网页为单一文件，并且适用于 Chrome 和 FireFox 等**众多浏览器**（mhtml是Chrome独占的格式）。对比 mhtml，SingleFile 会压缩代码（minified），自动移除未被使用的资源。

→ 查看详细

[GitHub - gildas-lormeau/SingleFile: Web Extension and CLI tool for saving a faithful copy of an entire web page in a single HTML file](https://github.com/gildas-lormeau/SingleFile)

---

3、Mozilla 改版了 MDN 网站，更加重视社区内容。首页在精选文章下直接放了「最近贡献」。包括他们的标识也是通过社区投票选出的。

![moz_blog_header_MDN-Intro.png](Scenes%20Weekly%20%2345.assets/moz_blog_header_MDN-Intro.png)

{上图：MDN 的新 logo}

→ 原文

[A new year, a new MDN – Mozilla Hacks - the Web developer blog](https://hacks.mozilla.org/2022/03/a-new-year-a-new-mdn/)

---

4、awwwards 公布了2021年度奖项，真是一群创意力十足的人。

![awww.png](Scenes%20Weekly%20%2345.assets/awww.png)

{上图：awwwards 奖杯}

→ 全部名单

[Annual Awards 2021 - Discover the best of the Web on Awwwards](https://www.awwwards.com/annual-awards-2021/)

---

5、从第4条出门左转就是东京 TDC 奖项。东京 TDC 评委有着更独特的眼光，[第三期](https://mp.weixin.qq.com/s/hAl8UML6iGDYWm0__JPUYQ) 提到的 GT MARU 也获得了网站方面的奖项（不是字体本身）。

→ 東京TDC賞2022

[東京TDC賞2022：受賞作品＋ノミネート作品発表｜NEWS｜Tokyo TDC](https://tokyotypedirectorsclub.org/news/tdc2022-results/)

---

6、99 designs 对144个国家超过一万名设计师进行了调研，每5名自由设计师就有1个在 angency 工作（应该指的是 按项目团体工作）。85%的设计师觉得，和客户有着共同的价值观——「合得来」比项目报价更为重要。后疫情时代，大家都比较继续看好设计的未来。

→ 详细数据

[Get a fresh take on the world of freelance – view the designer report.](https://99designs.co.uk/design-without-borders)

---

7、在 macOS 中打开检查元素功能，如下图。

![macOS.png](Scenes%20Weekly%20%2345.assets/macOS.png)

{上图：偏好设置中的一些界面并不是原生的}

这里面有着大量非 webkit 标准的 CSS 属性来适配系统 API，还能看到 react 的身影。Jim Nielsen 猜测可以从 Safari 那边的非标准更新来推测未来 macOS上 的功能。总之，是个有意思的事情。

→ Jim Nielsen Blog

[Inspecting Web Views in macOS](https://blog.jim-nielsen.com/2022/inspecting-web-views-in-macos/)

---

8、苹果的春季发布会没有 M2，但却迎来了M1家族最后一位成员 M1 Ultra。这颗把两枚 M1 MAX 「粘在一起」（UltraFusion 2.5D 封装，并不是新技术）的 SoC 有着恐怖的晶体管数量，能效完爆 12900K（DDR5），GPU 性能也超过了 RTX 3090……但老样子苹果只会给出这种几乎没有什么数值的曲线，连具体主频都没有提到。

![APPLE.png](Scenes%20Weekly%20%2345.assets/APPLE.png)

{上图：苹果官方发布的性能对比图表，并且只在底部小字注解中提到具体型号}

看似神乎其神，但是综合之前的 SoC 效能苹果貌似并没有说什么大话……等待上市后第三方性能评测。

→ Apple Newsroom

[Apple unveils M1 Ultra, the world’s most powerful chip for a personal computer](https://www.apple.com/newsroom/2022/03/apple-unveils-m1-ultra-the-worlds-most-powerful-chip-for-a-personal-computer/)

---

9、网络安全专家 Hoek 分享了提升 Windows Defender 效率的使用技巧。按照这位大哥的说法，只要你足够能折腾，Defender 完全是够用的。文章介绍了如何使用组策略开启 Microsoft Advanced Protection Service（MAPS）、防勒索、设置定时更新等等功能。

→ 原文

[Windows Defender is enough, if you harden it](https://0ut3r.space/2022/03/06/windows-defender/)

---

10、[第32期](https://designscenes.zhubai.love/posts/2076946627176427520)提到了 Apple Music 在艺人数据库方面的混乱，Jake D. 这次提到的是桌面端 AM 的搜索联想和导航问题，其中后者最令人困惑。

![AnimatedImage.gif](Scenes%20Weekly%20%2345.assets/AnimatedImage.gif)

{上图：AM 的导航演示}

AM 的导航是独立的，不会从一个侧栏项目返回到另一个项目，Spotify 则可以完成全局的返回。AM 这点确实做的很让人降低探索欲望。除此之外还有一些交互反馈不到位和加载慢的通病，AM 有不少的改进空间。

→ 原文

[CINNAMON | Apple Music’s User Experience Problem](https://cinnamon.agency/blog/post/apple_musics_ux_problem)

---

11、Substack 推出了 iOS App，这对于其他产品是一件平平无奇的事，但是对于 Substack 这个邮件订阅起家的产品来说，又有很多不同的意义。 就像正常理解一样，Substack App 集成了你的订阅内容，之后可以不必翻阅邮件，直接在 App 上阅读。但是——

![subs.png](Scenes%20Weekly%20%2345.assets/subs.png)

{上图：Substack 新用户引导流程}

Substack 注册必须是真实邮件，不支持匿名加密的邮箱更不支持手机号，维持住了底线（但不妨期待下未来短信服务的 RCS 升级？）。啧啧称赞的下一步就蚌埠住了，检查邮件，依然是链接登录。于是我在**桌面端**浏览器打开邮件链接时，登录流程就卡在了这里。不是很懂 Substack 为什么默认用户会在手机上打开链接……但本质一段带有token的链接，复制粘贴到手机上可以继续登录。这里改为一串登录验证码更通用。

后面就是引导开启通知和联动 Twitter 账户信息。你能看到你的 Twitter 关注者都关注了哪些作家。可能前有 Revue 的先天优势，Substack 也比较急。这些都是邮件所做不到的事情，正如官方所说，Substack 要开始构建自己的创作者生态。创作者不会被聚合平台利用沦为流量工具，平台只会利用网络外部性（官方说 Substack 的付费用户会有2.5倍的意愿付费订阅更多创作者）来增加创作者收入。

至于[有人提到](https://twitter.com/bmorrissey/status/1501568928799244290)，Substack 会给 App 用户默认取消邮件推送，我没有看到🤔。App 整体是为了读者方服务的（没有创作者发布功能），但只能免费订阅，付费订阅还需在网页上实现以规避苹果税。

→ 官方文章

[Introducing the Substack app](https://on.substack.com/p/substackapp)

---

12、一个新的2D图像3D感知模型 StyleNeRF，比起之前的GAN支持分辨率更高，伪影更少更自然。

![pipeline_image.png](Scenes%20Weekly%20%2345.assets/pipeline_image.png)

{上图：演示图}

→论文

[StyleNeRF: A Style-based 3D-Aware Generator for High-resolution Image Synthesis](http://jiataogu.me/style_nerf/)

---

13、POCKIT 是一个模块化PC项目，在一块PCB上搭配不同模块可以实现各种中继和终端功能。作者已开发三年，得益于 USB-C 24pins 提供的丰富总线策略。现在已经有完整的演示视频了。

![pocket.png](Scenes%20Weekly%20%2345.assets/pocket.png)

{上图：POCKIT 能实现的组合}

→ 官网

[Project Pockit](https://pockit.ai/)

---

14、hoooooooorse，Stupid Hackathon 产物。马腿能有多长呢。

→ endless.horse

[hooooooooooooooooooooooooooooooooooooooooooooooooooooooooorse](http://endless.horse/)

---

15、上一期讨论了GIF文件的帧延迟处理，这次有全面的GIF格式科普。

→ You Don't Know Gif - An analysis of a gif file and some weird gif features

[You Don't Know Gif - An analysis of a gif file and some weird gif features](https://blog.darrien.dev/posts/you-dont-know-gif/)

---

# 劳逸

![99fab11241664812a1cdbb9f0f4305eb.jpeg](Scenes%20Weekly%20%2345.assets/99fab11241664812a1cdbb9f0f4305eb.jpeg)

{上图：艾尔登法环游戏内截图——和金面具老师「合影」}

在艾尔登法环度过了100小时后的感受：它有着足够多的内容去沉浸和探索，但质量并不总是上乘；它的个别 Boss 战斗足够恢弘，但是大多 Boss 只想让它赶紧过去；它的评价足够撑起90+/100分的门面，但是缺点也不是没有，比如一些按键交互问题和后期一些地牢/怪物设计的乏味。这段时间很充实、满足。

---

# 映像

现实拟像放映——

![c184994570ec438cb468b3264043e472.jpeg](Scenes%20Weekly%20%2345.assets/c184994570ec438cb468b3264043e472.jpeg)

{上图：鞋底与键盘键帽}

©Gab Bois

---

喜欢本文的话，欢迎分享、订阅。

第 44 期请[在此查看](./Scenes Weekly #44.md)。

本次封面使用了 Cormorant Garamond 字体，图形灵感来自 Elden Ring。