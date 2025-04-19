# Scenes Weekly #34

2021-12-13

\> 设计视角下的世界——

第 33 期请[在此查看](./Scenes Weekly #33.md)。

本期出现：Google Font Knowledge、Modern fluid typography editor、UI Fund、Cash、Online Spyware Watchdog、Scan of Month、Web3、Modern Design for Wikipedia、Emoji Frequency、Quill、隐私政策与用户协议生成、Alexa、Fable

如有格式异常建议点击最上方「在浏览器中访问」。

---

# 微博

1、Google Font 上线了 Knowledge 板块，从介绍字体、选择字体到使用字体做了详尽的入门介绍，并附带了一般术语介绍。

![58caac17ff6346e6a4ba48119f6d54da.png](Scenes%20Weekly%20%2334.assets/58caac17ff6346e6a4ba48119f6d54da.png)

{上图：Google Font Knowledge 说明}

→ 学习

[Fonts Knowledge - Google Fonts](https://fonts.google.com/knowledge)

---

2、上次讲 Material Design 3 的[第28期](./Scenes Weekly #28.md)里提到了多设备字体缩放的事情。Adrian Bece 做了一个 Modern fluid typography editor 工具，设置好参数后使用 clame() 函数去适配不同不宽度。

![9a7edbb1077741f1aa38f248c10f62f5.png](Scenes%20Weekly%20%2334.assets/9a7edbb1077741f1aa38f248c10f62f5.png)

{上图：Modern fluid typography editor 曲线展示}

→ 工具地址

[Modern fluid typography editor](https://modern-fluid-typography.vercel.app/)

---

3、Chrome 在 web.dev 上宣布成立一个 UI Fund，旨在资助支持那些从事设计工具、CSS 和 HTML 相关项目。 顺藤摸瓜发现了 Open UI 这个社区项目，项目还处于初期，它想为各个网页控件制定统一的标准，比如一个标准的 Dialog （对话框）控件应该包含哪些内容，这些内容也将会被统一命名，并会拿一些常见的 Design System 举例。

→ UI Fund

[The UI fund](https://web.dev/ui-fund/)

→ Open UI

[Home](https://open-ui.org/)

---

4、Build for Mars 这期分析了 Cash 这款热门移动支付应用。Cash 宣称自己是 The easiest way to send, spend, bank, and invest。然而却在新用户注册流程中出现了一些问题。比如没有软着陆页面、容易分散注意力的按钮，昵称不可用时没有提供额外任何建议、错误引导获取敏感权限、没提供流程进度等。

![b4830498e2ec431d8a538542fa17c9b6.png](Scenes%20Weekly%20%2334.assets/b4830498e2ec431d8a538542fa17c9b6.png)

{上图：Cash 应用内一些优化点的展示}

虽然这跟实际的 easiest way 行为没什么关系，但是可以看出 Cash 的简单易用理念已经过多渗入到了设计里面，易用和简洁的界面并非绝对处于等号的两侧。 我们在 Mobbin 上可以看到今年六月收录的 Cash 页面，半年来在注册流程上只优化了姓名填写那里。剩下还有拉新奖励的机制优化。

→ 详见

[A UX case study on Cash App ✌️](https://builtformars.com/case-studies/signing-up-to-cash-app)

---

# 摘录

> 几乎所有做图文视频产品的内容运营，好像都把默认用户当成老色批。可气的是，他们通常还是对的。

—— 刘言飞语《[一些碎片观察和想法 202112](https://mp.weixin.qq.com/s?__biz=MjM5NDkyNTUzOA==&mid=2657925061&idx=1&sn=dddbb8d5a0e2f0332782f71fa2e3e42a&scene=21#wechat_redirect)》

---

# 杂事

1、Online Spyware Watchdog 这个网站披露了那些日常使用的应用里 spyware 的一面。该网站对 spyware 标准极其严格，基本未经用户同意的任何自发行为（包括自动升级）都会列入警告。即使是以隐私标榜的 DuckDuckGo 也被判定为 Possible Spyware。

→ 看看你在使用哪些间谍应用

[Catalog - Spyware Watchdog](https://spyware.neocities.org/articles/index.html)

---

2、Scan of the Month 每月会对一些物品进行三维CT扫描，上个月是乐高人仔系列，这个月是 Airpods 的1代到 Pro 再到3代的进化历程。

![proct.png](Scenes%20Weekly%20%2334.assets/proct.png)

{上图：Airpods CT下的结构图}

原文还配有解说文字。但不知道为什么没有往月的扫描结果归档……

→ 查看原网站

[Scan of the Month: you won't believe what you see inside objects with a CT Scanner.](https://scanofthemonth.com/)

---

3、在[上一期](./Scenes Weekly #33.md)本通讯提到了一篇[工程师视角的 Web3 分析](https://www.psl.com/feed-posts/web3-engineer-take/)，「很遗憾」这次依然会继续揭开 Web3 的面纱，Press X to Doubt！

Jay Pinho 在他的 Substack 专栏 networked 里表示出他的疑问：

- 如今的技术/协议的关键细节是无法处理凭证与去中心化的；例如去中心化DNS服务商 Ethereum Name Service（ENS），所有ENS域名都在其根节点下注册，根节点资产使用多重签名协议持有，但其密钥由值得信赖的社区个人持有，剩下的承诺依旧归于道德层面。
- NFT 的所有权依赖于卖方制定的规则，比如 NBA Top Shot 就有着自相矛盾的说明，一边说您购买的珍惜瞬间是独一无二的，是有NBA官方许可的。一边又偷偷声明您无权分发、复制以及对材料的任何商业化行为……您连解释权都没有。
- NFT 的盗窃风过于泛滥，甚至有这么一个 [Twitter 账号](https://twitter.com/NFTtheft)专门记录这些无耻的行为。NFT 本质自是一个链接🔗。Jay 举了一个例子：就像一张纸条，上面写明了在高楼大厦中的哪个公寓的某个房间里，可以寻找到你购买的那个「艺术品」。这个公寓可已被夷为平地，也可能快了。
- 智能合约的问题，详见[上面提到的文章](https://www.psl.com/feed-posts/web3-engineer-take/)。
- 一个有意思的对比：App Store 是2008年7月推出的，中本聪的白皮书是2008年10月发布的，如今 App Store 的蓬勃发展，其应用生态一度走在垄断边缘，影响着十几亿人的生活。而另一边却还在从华尔街借来「万物皆可证券化」的话术格式，关心 Web3 也只是关心它背后能帮自己赚多少钱，哄抬 NFT 也不过是扩展市场规模以提高早入局的红利。

→ Pinho 还在文章末尾还列出了一份阅读清单

[Web3? I have my DAOts](https://networked.substack.com/p/web3-i-have-my-daots)

---

4、Modern Design for Wikipedia 是一个浏览器扩展插件，优化了现有的 Wikipedia 页面排版。

![b6b3ff8c-9ee2-4f61-966a-7b20161338a5.jpeg](Scenes%20Weekly%20%2334.assets/b6b3ff8c-9ee2-4f61-966a-7b20161338a5.jpeg)

{上图：优化后的wiki界面，目录整体放到了左边}

并且可以依据个人偏好，设置衬线还是非衬线字体、字号、字间距、行宽、以及包括深色模式在内的五种主题。该插件完全免费且支持 Chrome、FireFox 和 Edge。

作为一个曾经试图重构过 wiki 界面的人，我很清楚作者开发者为此已经付出多少努力。但其实并没有对 wiki 本身结构做过多调整，比如 Quick Facts 部分依然有优化的空间。

→ 安装

[Modern for Wikipedia](https://www.modernwiki.app/)

---

5、Unicode 联盟公布了2021年emoji 使用频率排行，😂 依然是第一名。这篇文章还对比了疫情前后的 emoji 频率变化。

![截屏2021-12-09 16.11.00.png](Scenes%20Weekly%20%2334.assets/%E6%88%AA%E5%B1%8F2021-12-09%2016.11.00.png)

{上图：2019年和2021年的前十名使用频率emoji对比}

可以看到2019年前十名里的💕被带人脸的🥰替代，后者是2018年最新更新的一波表情里的，戴口罩😷的emoji使用排名并没有明显上升（186 → 156名）。

→ 详见

[Emoji Frequency](https://home.unicode.org/emoji/emoji-frequency/)

---

6、Twitter 去年这个时候收购 Squad，公告称服务将在24小时后关闭；今年收购了 Quill 后预留了4天迁移，是不是应该「称赞」一下呢？我对 Quill 不太了解，但是大家都知道 DM 一直是 Twitter 的短板，在推出了各种会员服务后，完善 DM 甚至之前提到的社区功能也顺理成章。

![image.jpeg](Scenes%20Weekly%20%2334.assets/image.jpeg)

{上图：Twitter Logo + Quill Logo}

→ 关闭公告

[https://quill.chat/updates/2021-12-07-quill-twitter/](https://quill.chat/updates/2021-12-07-quill-twitter/)

---

7、在 V2EX 上看到，用户 @crazyorr 以常年和各个商店审核人员斗智斗勇的经验，开发了隐私政策和用户协议生成工具，只需要填写产品名称、开发者名称、产品功能、联系方式信息就能生成两段文本。目前开发者还在根据论坛回复不断添加新的审核点。当然，协议写的再百密无疏，也要执行到位呢，否则说不定什么时候被抽查当做豆瓣下架类似新闻背景板。

→ 论坛原帖

[国内上架 APP 必备利器：隐私政策生成工具 - V2EX](https://www.v2ex.com/t/819045)

→ 隐私政策生成

[toolbox](https://toolbox.yolo.blue/#/privacy-policy)

→ 用户协议生成

[toolbox](https://toolbox.yolo.blue/#/terms-and-conditions)

---

8、The Next Great Game: Politicians vs Tech Companies

[The next great game: Politicians vs tech companies](https://www.gzeromedia.com/the-next-great-game-politicians-vs-tech-companies)

标题即为概括。

---

9、流量统计网站 Alexa 将于明年五月一日下线，曾经依靠工具栏和插件为基础设施的站长必备「伴侣」，距离 PageRank 不再开放的六年后，在如今隐私时代已是明日黄花。

Alexa 的创始人 Brewster Lurton Kahle 在1996年同时创造了 Alexa 和 Internet Archive。

→ 公告原文

[We retired Alexa.com on May 1, 2022](https://support.alexa.com/hc/en-us/articles/4410503838999)

---

10、动效工具&平台 Fable 历经三年测试打造后，最近正式上线。A轮1500万美元由红点创投（Redpoint Ventures）领投。Fable 之前的点是使用网页工具可以轻易做出粒子相关动效，现在他们更加注重降低动效制作门槛。比如下图他们自带的丰富预设：

![fable - lib@2x.png](Scenes%20Weekly%20%2334.assets/fable%20-%20lib@2x.png)

{上图：Fable 预设合集}

实际使用时我发现一个 Comtroller 功能，图示看样子像在控制相机。但在「帮助文档」里很难找到 Controller 相关的介绍让我有点受挫……

→ 官宣

[Fable launches with $15M Series A from Redpoint Ventures](https://medium.com/fable-motion/fable-launches-with-15m-series-a-from-redpoint-ventures-f0ffbe0b2817)

---

# 劳逸

![342b52c07371496e8645b89248a6c427.png](Scenes%20Weekly%20%2334.assets/342b52c07371496e8645b89248a6c427.png)

{上图：光环无限中的士官长与"武器"}

《真·女神转生V》几乎变成了我的日常游戏，今年游戏时间进一步缩短的情况下断断续续玩了一个多月也没玩完。饱受媒体赞誉的《光环 无限》战役也因为 XGP 无比恼人的体验变得一团糟。我在第31期预测的TGA奖项基本折戟。平淡的一周。

---

# 映像

现实拟像放映——

![9f8a876c366c4cf99919a3550836a5ab.png](Scenes%20Weekly%20%2334.assets/9f8a876c366c4cf99919a3550836a5ab.png)

{上图：风吹起了落叶，遮住了路边一只鸽子头部}

Spectrum Photo Creatures in the Air Award & Affinity Photo People's Choice Award:

I guess summer's over (in Scotland).

© John Speirs/Comedy Wildlife Photo Awards 2021

---

本次封面使用了 Marle (Trial) 字体。