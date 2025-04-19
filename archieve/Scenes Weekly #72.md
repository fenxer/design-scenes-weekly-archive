# Scenes Weekly #72

2022-10-03

\> 设计视角下的世界——

第 71 期请[在此查看](./Scenes Weekly #71.md)。

本期出现：

- iPhone 屏幕像素宽度吐槽
- Twitter 已编辑
- 坐看互联网
- 网络页面年鉴
- 其他：iOS 备忘录URL Scheme、WordPress 脱离服务器 demo、OG App 下架风波、Winamp 客户端、Substack Reader 网页端更新、躺平孰对错、猫咪落体物理、Windows PWA 应用更新、Stadia 拜拜

如有格式异常建议点击最上方「在浏览器中访问」。

---



本来这期想拖到放假后再发，但是竹白的推送上周又出了些问题🥲，导致一些订阅者延迟收到了邮件，特此说明一下。

而且这周也没什么设计类的信息，不过来都来了，#轻松一刻 再开。

下周不出意外不会更新。

欢迎上周的新订阅者，祝所有订阅者都能有一个愉快的假期。

---

# 轻松一刻

1、你可能已经知道 iPhone 14 系列尺寸有多奇葩：

> 6.1寸的iPhone 14 宽度 390px，iPhone 14 宽度 393px；

> 6.7寸的iPhone 14 Plus 宽度 428px，iPhone 14 Pro Max 宽度 430 px；

6.1 寸差了 3 像素，6.7 寸差了2 像素，响应式设计永驻我心。

![meme.png](Scenes%20Weekly%20%2372.assets/meme.png)

{上图：一个 meme 而已}

→ [吐槽灵感原文](https://polypane.app/blog/thanks-i-phone-14-designing-for-device-sizes-is-dead/)

---

2、Twitter Blue 展示已编辑推文状态，会在日期附近带有一个「笔」的图标。

![TWITTER.png](Scenes%20Weekly%20%2372.assets/TWITTER.png)

{上图：Twitter 第一条已编辑的推文}

可点击时间查看编辑历史，更改后似乎所有数据会重置。与删了重新发一遍的区别在于，这可证明是编辑过的，也就是编辑行为自身。

→ [原推文](https://twitter.com/TwitterBlue/status/1575590534529556480)

---

3、一个坐看互联网的网站 [realtime.info](http://realtime.info) 可以不停地刷新一些实时数据，分为图片、信息和数据三部分，并且可以调整刷新速率以及是否显示 NSFW 内容。一不留神，盯着几分钟过去了。

![截屏2022-10-01 15.04.06.png](Scenes%20Weekly%20%2372.assets/%E6%88%AA%E5%B1%8F2022-10-01%2015.04.06.png)

{上图：网站截图}

→ [看看](http://realtime.info/)

---

4、Web Almanac 是 HTTP Archive 出品的一份年度网页报告，搜集了超过 800 多万网站数据，涵盖了页面内容、用户体验、内容发布和分发等领域。

在网页字体一节中，能看到 64.5% 网站都在使用 Google Fonts 托管服务，虽然 2022 年有所下降。

![webfont-usage-by-service.png](Scenes%20Weekly%20%2372.assets/webfont-usage-by-service.png)

{上图：Webfont usage by service 柱状图统计}

可变字体的使用率也比去年高出一倍之多，但也只有28%左右。这其中 97% 也是使用 Google Fonts 上的可变字体，87% 都只使用了 wght 轴（调节字重）。可变字体的网页应用之路还很远。

无障碍一节中，有着足够颜色对比度（WCAG 2.X 标准）的网站仅占 22.9%，连续四年增幅 1% 都不到。

→ [你可能会关心更多数据](https://almanac.httparchive.org/en/2022/)

---

5.1、iOS 备忘录也是有 [URL Scheme](https://developer.apple.com/documentation/xcode/defining-a-custom-url-scheme-for-your-app) 的：

```objectivec
mobilenotes://showNote?identifier=UUID
```

→ [这篇文章](https://www.macstories.net/ios/creating-lock-screen-widgets-for-specific-notes-via-the-apple-notes-url-scheme/#fn-70650-1)介绍了如何获取每篇备忘录的 UUID。



5.2、得益于 WebAssembly（WASM）技术，WordPress 一个小 demo 演示了如何脱离 PHP 服务器运行。由于 MySQL 不支持，但有插件使数据库支持 SQLite3。Demo 演示了正常发布文章，但还是有不少功能限制。

→ [Client-side WebAssembly WordPress with no server](https://make.wordpress.org/core/2022/09/23/client-side-webassembly-wordpress-with-no-server/)



5.3、OG App 是一款第三方的 Instagram 应用，可以自定义是否显示原本 Ins 上多余的功能和内容，包括广告。他们在 Android 上逆向工程了 Ins 的私有 API，并采用了一些特殊方法才能登录应用（团队[承诺之后会改进](https://twitter.com/TheOGapp_/status/1574861237963223040)）。但 Meta 坐不住了，[封禁](https://twitter.com/TheOGapp_/status/1575265782094647296)了他们团队每个人的 Facebook 账号，应用也从 App Store [被强制下架](https://twitter.com/TheOGapp_/status/1575217497011200001)。这个事件里，对私有 API 获取的数据处理是一个灰色地带，但是从先有蛋还是先有鸡的角度来看，如果不是群众苦 Ins 已久，也不会有 OG App 这样的应用诞生。



5.4、上周才发现，Winamp 的客户端居然[长这样子](https://www.winamp.com/player/)……

📮回溯：[winamp 皮肤铸造](https://designscenes.zhubai.love/posts/2117545871552929792#:~:text=%E5%9B%BE%EF%BC%9A%E7%BB%8F%E5%85%B8%E7%9A%AE%E8%82%A4%7D-,%E5%AE%9E%E9%99%85%20Winamp%20%E7%9A%84%E4%BA%A7%E5%93%81%E5%91%A2,-%EF%BC%9F%E6%97%A0%EF%BC%8C%E4%BD%86%E4%BE%9D%E6%97%A7)



5.5、Substack Reader [网页端更新](https://on.substack.com/p/new-web-reader)，加入了键盘快捷键导航，以及第三方 RSS 订阅。



5.6、一些员工悄悄辞职，是员工问题还是老板问题呢？哈佛商业评论（HBR）[一篇文章](https://hbr.org/2022/08/quiet-quitting-is-about-bad-bosses-not-bad-employees)收集数据显示了国外员工躺平（quiet quitting）趋势。正如你所预料的那样，对领导评价越高的员工群体，躺平率越低。90-100分段的领导手下员工仅有 3% 躺平，62% 的人保持上进心态。而到了 1-9 分段的领导，手下员工 14% 都在躺平，仅 20% 的有上进心，剩下 67% 的人都是中立心态，过一天是一天。当然领导人好不好并不是影响员工心态唯一因素，但是将躺平完全归咎于员工的领导，应该先审视自己和组织。 



5.7、1894年摄影先驱 Étienne-Jules Marey 展示了猫咪自由落体的影片。片中的猫从倒挂的状态，在落下时先从头部开始翻转，继而转动身体，最后四肢着地。到现在已经不会说猫翻正反射在挑战角动量守恒，反而猫猫的身体结构来仿生学带来了很多课题。The Atlantic [这篇文章](https://www.theatlantic.com/science/archive/2022/09/falling-dropped-cat-reflex-physics/671424/)在讲猫的摔落极限高度是多少，[研究表明](https://pubmed.ncbi.nlm.nih.gov/3692980/)猫从 6-7 层楼以及更高处掉落，受伤率逐渐趋于稳定（← 仅仅是搜集案例，不是拿猫做实验）。虽然这些都是残忍的现实，但好在高楼综合症的猫猫生存率都超过 90%（但还时会受伤的😥），与人类对比这是惊人的数值。

一个细节是，猫从7层以上高度降落后，高速下落的失重感会带来一种「愉悦」，让猫猫放松腿部肌肉，这导致高层坠落的猫受伤经常是躯干和下巴，而不是四肢。

真心祝愿所有的猫猫都健健康康。



5.8、微软想帮助 PWA 开发者让TA们的程序看起来更像原生应用，允许开发者定义默认标题栏。Web 应用的流行或许该反思未来系统组件的意义。

→ [原文](https://blogs.windows.com/msedgedev/2022/09/27/closing-pixel-gap-native-web-window-controls-overlay/)



5.9、Stadia 的员工[知道自己部门解散的消息没比吃瓜群众早多少](https://9to5google.com/2022/09/29/stadia-employees-shutdown-meeting-harrison/)。当前云游戏体验一直不算好，很多玩家已经在设备和显示延迟外不想再新增延迟要素。但是数据告诉高管们这东西有前途，于是入场不撞南墙不回头。和字节的 Pico 一样，有点像斗兽棋中的「鼠吃象」，老鼠作为大象下的食物链底层，却也能决定大象的生死。

---

# 重读HIG（十二）

本节是重读 Human Interface Guidelines 系列连载第十二期，目的为温故知新和跟进新内容。 为避免篇幅过长，不会一次发布太多，之前内容已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上。

HIG 临时更新了 Charting data 和 Collaboration and sharing 两节，好一个偷tóu袭xī，下次写。

## 实时收看应用（Live-viewing apps）

我没记错的话，本节内容和 [Right to Left](https://developer.apple.com/design/human-interface-guidelines/foundations/right-to-left) 一样是新增加的。

HIG 这里的 live-viewing 包括了直播和新闻播放等实时内容，所以没有简单地使用 live-streaming。Live-viewing 与 Video-on-command（VOD，视频点播）相对。

针对 tvOS   实时内容的特点，HIG 有如下建议：

- 突出实时内容，使之易于访问。点击一次或者不点击即播放，但需要注意默认音量、网络环境等实际情况；
- 实时内容要和 VOD 内容区分开，常见的比如一个 LIVE 标识；
- HIG 推荐实时内容也需要进度条，以便显示剩余时间。又一点不解的是，如果是为了回看倒是可以理解，进度的话大部分直播进度都会在最右边。即便是 Apple 自家的发布会页面也没有显示剩余时间；
- 观众离开实时内容观看有时并不带表结束了观看，此时可以继续播放背景音频。但如果观众划走、关闭或者切换到别的内容页面，判断结束观看时，可关闭音频，停止播放实时内容；

后面还有EPG（节目单）和云 DVR 的介绍……这个实在是有点陌生，详见原文吧。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/live-viewing-apps)

## 加载（Loading）

加载这一节没有新的内容。

- 尽快展示内容是最优先的事；
- 如果加载时间比较长，可以展示加载进度和时间；
- 如果加载时间很长，可以尝试显示一些额外可供消遣的信息；
- 自定义加载样式可以带来更沉浸的体验；

HIG 唯一提起的是，尽量避免在 watchOS 中显示加载。推测这是鉴于 Apple Watch 的「表」属性，让人对时间更敏感，从而容易损害 Apple Watch 产品的认知。

如果是在游戏中，加载的相关事项可能会更多，需要权衡性能与体验。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/patterns/loading)

---

# 摘录

这周看过的一些——

> 张一鸣敢于用自己信任的人跨界做新业务——即使没有直接从业经验。报纸广告业出身的张利东管商业化、今日头条产品负责人陈林管大力教育，都是如此。2019 年初，原战略投资部负责人严授兼任朝夕光年负责人。他在一年后全职负责字节游戏业务。

> 多位字节员工认为，2015 年入职的严授是 “特别咨询公司风格” 的人，聪明、理性，“打交道时场面上的礼节都做到位”。开会沉闷的时候，他会说几句俏皮话维持场面——尽管 “笑话不好笑”。

> 一位前员工评价严授是 “典型的老字节人”。他听严授讲过如何设计 OKR，“正反举例，讲得很实在”；为人朴实，不端架子。一位和严授有业务往来的前字节人士感知到的严授也信奉 “大力出奇迹”，“觉得从前的成功经验可以在各个领域复制，觉得自己先进，对各个领域原来建立起来的门槛是不尊重的，可以把一切颠覆、重建、提效、量化。”

> 严授也不是游戏玩家。一位朝夕光年发行线员工评价严授 “关注点比较宏观”，看的是全行业数据，没听他评价过游戏好不好玩。一位研发员工回忆，跟严授一对一交流时有 “搭不上线” 的感觉：他聊到在玩一款当时很火的游戏，严授没有反应，“看着像没听说过”。

—— 晚点LatePost - [复盘字节游戏：氪了几百亿元，没算出人性](https://mp.weixin.qq.com/s/g__Gdfqmqt4BtF-Tnripjw)

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

![XENO.png](Scenes%20Weekly%20%2372.assets/XENO.png)

{上图：异度神剑3}

放假了——终于有时间开始沉浸异度神剑3了——

但收藏版还没到货，急。

等玩完再谈。

---

# 映像

现实拟像放映——

![294462600_203356908687460_508230228593553602_n.jpeg](Scenes%20Weekly%20%2372.assets/294462600_203356908687460_508230228593553602_n.jpeg)

{上图：画作 The vintage festival 中的带花环拿着火炬的女性，被修整为在公交上握住把手}

[Alexey Kondakov](https://www.instagram.com/alksko/) 的超现实主义摄影总是让人看不厌。

原作：[Lawrence Alma-Tadema](https://artsandculture.google.com/entity/m073zs) 的 The vintage festival

---

# 温故

→ [Scenes Weekly #23](https://mp.weixin.qq.com/s/trmup73B9Qw2MNgBiLmLIg)

- W3C 网站重设计
- 苹果秋季发布会的可变字体
- 行长对阅读速度的没有很大影响
- Monotype 收购了 Hoefler&Co
- 推文内容生成图片的网页工具 Poet.so
- Apple v. Epic 看法
- Mailchimp 被收购

---

喜欢本文的话，欢迎分享、订阅。

第 71 期请[在此查看](./Scenes Weekly #71.md)。

本次封面使用了 Quicksand 字体。