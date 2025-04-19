# Scenes Weekly #67

2022-08-29

\> 设计视角下的世界——

第 66 期请[在此查看](./Scenes Weekly #66.md)。

本期出现：

- 新世代演示文稿工具下的幻想
- Artboard Studio 发展
- 重读 HIG（八）
- CSS :has()伪类走向舞台前
- 人工智能生成图像事情三则
- 科隆游戏展观后浅谈
- 其他：用户调研免费入门电子书、百味来 Spotify 歌单、Design the Next iPhone、Great Landing Page Copy 人性化文案展示、Steam Deck 手册

如有格式异常建议点击最上方「在浏览器中访问」。

---

你可能已经看过这个新闻——2021 年 2 月，一位全职父亲 Mark 发现自己儿子的私处有些异样的肿胀，便使用 Android 手机拍摄了腹股沟处，一方面记录病情发展，另一方面为第二天早上的视频问诊准备材料（由于 COVID-19）。**在照片的帮助下**，医生诊断后开了抗生素，症状很快缓解了。但网络另一边的 Google 可不这么认为，这些照片被上传至 Google 相册后触发了警报，被标记为儿童性虐待内容（CSAM）。Mark 包括 Google Fi（虚拟手机号）在内的所有 Google 服务被冻结，严重影响了他的数字生活和本人声誉。你可以在[纽约时报](https://www.nytimes.com/2022/08/21/technology/google-surveillance-toddler-photo.html)读到最为详细的报道（或者国内[品玩的报道](https://www.pingwest.com/a/269282)）。

感叹的是，在警方取证调查后的一年多时间，Mark 被证明是清白的，然而 Google 依然拒绝为 Mark 恢复服务。这个事件就像 Apple 当初推出 [Expanded Protections for Children](https://www.apple.com/child-safety/) 一样复杂，道德、科技与人性交织在一起，只有无尽的争议。

> → 回顾：本通讯曾在[第 17 期](https://mp.weixin.qq.com/s/Pg3Yc7iopK8hbHJ9TcWG3A#:~:text=%E8%8B%B9%E6%9E%9C%E6%89%80%E8%AF%B4%E7%9A%84-,CSAM,-%E6%8A%80%E6%9C%AF%E5%90%A7%E3%80%82)介绍了更为谨慎的 Apple 限制 CSAM 的措施（Apple 在设备上就开始扫描了），并在[第 19 期](https://mp.weixin.qq.com/s/MXedICedQ4TIBTcXbx3kog#:~:text=%E4%B8%8B%E8%8B%B9%E6%9E%9C%E7%9A%84-,NeuralHash,-%E6%A8%A1%E5%9E%8B%E8%BE%93%E5%87%BA%EF%BC%8C%E5%8F%91%E7%8E%B0)提到了针对 NeuralHash 算法的二次原像攻击风险。

舆论放大了 AI 算法识别的误报率所产生的不良后果，但却没有引起 Big Tech 公司的更多重视。回归事件本身，不理解铁证之下 Google 发言人为何依然坚持不恢复误报人的服务。科技本应为人服务，但现在却作为审判的冰冷利剑——顺便看了一眼我的 QRCode 脚镣。

这周 Mudeg 对 Twitter 的指控使后者进一步陷入舆论漩涡，但目前只是Twitter 与 Musk 的「衍生剧」。如果感兴趣，一如既往你应该看看[Matt Levine](https://www.bloomberg.com/opinion/articles/2022-08-23/amc-goes-ape) 的有趣报道。

对了，我最近新开的**重读 Human Interface Guidelines***一栏已在* Craft 上整理完一部分内容，可以[点这里访问](https://www.craft.do/s/fH49oLBCFdJO4l)。在 Patterns 一章写完应该还会提醒一下，所以可以放心跳过重读 HIG 这一栏了（？）

最后，欢迎上周的新订阅者。感谢所有订阅者的支持。

---

# 杂事

**Cyma Curves 更新**：[第 65 期](https://designscenes.zhubai.love/posts/2170801615631011840#:~:text=%C2%A0%E4%BB%8B%E7%BB%8D%E4%BA%86-,cyma%20curves,-%E8%BF%99%E4%B8%80%E5%BB%BA%E7%AD%91)介绍了 cyma curves 的数学原理，后来有 [Design Lobster](https://designlobster.substack.com/) 的读者在 CodePen 中做出了一个该曲线的生成器，并可直接复制或下载 SVG。好啊！

[Cyma Curve Generator](https://codepen.io/os/pen/eYMKVqd)

---

1、演示文稿本质是叙事工具，只不过把当时幻灯机上的每页薄纸电子化。PowerPoint 的单页制作模式几乎凝固了我们的思维，甚至将演示文稿等同于”PPT”。换角度看当前 [Tome](https://beta.tome.app/)、[Chronicle](https://chroniclehq.com/) 和 [Gamma](https://gamma.app/) 等新兴的 storytelling 工具，都在突破内容结构的表现形式，并辅以更易上手的交互和舒适的视觉。

![rojector.png](Scenes%20Weekly%20%2367.assets/rojector.png)

{上图：两种透镜式投影仪。想起了我的小学老师，经常在调整灯箱上的纸张和镜片角度}

最先有类似感受的是使用 [Overflow](https://overflow.io/)，当时还在 beta 测试期。Overflow 做的事情很简单，把导入画布的元素连接起来，不仅无需自己画箭头，还可以存储切换多种样式。添加说明文字也变得非常简单，在演示时，使用方向键可以顺滑地移动到下个界面。不使用 Overflow 能实现这个工作流吗？可以，但是可能需要耗费额外精力，效果也不如人家流畅。Overflow 的工作看起来就像是交互体验的先进封装（Advanced Packaging）。这种趋势在之后愈发明显。

新出现的 **Gamma** 看起来更加回归演示文稿，加入了一些常见的图表模板，也支持自定义母版（theme），可以在浏览器中直接演示（present）。对此我有一些联想，Gamma 其实是可以兼容我这篇newsletter 内容，甚至在传递信息的接受率层面上会做的更好。上期最后我写了 [newsletter 历史回顾](https://designscenes.zhubai.love/posts/2173339109634928640#:~:text=5%E3%80%81-,Newsletter,-%E7%9A%84%E7%83%AD%E6%BD%AE%E4%BC%BC%E4%B9%8E)，所以我更想试试一种纯粹的 newsletter 形式，比如你每周收到一本这种小册子的话——

![mag.png](Scenes%20Weekly%20%2367.assets/mag.png)

{上图：把上期一部分内容变换为了 A4 双开横版杂志的排版实验}

——啊，梦醒了。

---

2、 **Artboard Studio** 最早（2018 年）专注于产品 mockups 的快速成型出图，与其他 mockups 网站不同的是，它可以在线自定义 mockups 内元素的位置。之后团队在 Artboard Studio 2.0 中（2019 年）加入了品牌系统，将品牌作为设计组件嵌入到设计图中，并可以实时协作。2020 年 Artboard Studio 可以制作动态的 mockups，添加了时间轴和关键帧。然后今年他们开始专注将 Artboard Studio 宣发为动画工具了……

![AS.jpeg](Scenes%20Weekly%20%2367.assets/AS.jpeg)

{上图：Artboard Studio 投放在 Product Hunt 的图片，上面写着 Design like Figma, animate like AE}

实际体验了一下，画板性能已经贴近 Figma，右边面板也基本和 Figma 统一了交互。点击 recording 图标时，输入框右边会变成代表关键帧的紫色菱形。作为单画板式动画工具，整合度比 Figma 插件（例如 [Motion](https://www.figma.com/community/plugin/889777319208467032)）高上不少，并且额外增加了 Transform Effects

另外，mockups 功能也依然有保留。虽然没有 [Rive](https://rive.app/) 的骨骼和 Mesh 那样强大，但尚且够用。遗憾的是没有找到导入 Figma 文件的选项。

顺便一提，[Device Mockups](https://deviceframes.com/) 这个工具做的事和早期 Artboard Studio 很像。

[Artboard Studio: Design and Animate Like Never Before](https://artboard.studio/)

---

3、Jan Dittrich 写了一本免费的电子书 ***A Beginner’s Guide to Finding User Needs***，作为用户动机、活动和需求的定性研究入门指南。内容详实，例证优先。在他的[写作风格指南](https://urbook.fordes.de/contributing/)里也提到了尽量少用不常用的术语，在入门方面下足了心思。由于时间和精力原因没怎么读……但我已经决定时刻「准备再次入门」！

![A Beginner’s Guide to Finding User Needs.png](Scenes%20Weekly%20%2367.assets/A%20Beginner%E2%80%99s%20Guide%20to%20Finding%20User%20Needs.png)

{上图：A Beginner’s Guide to Finding User Needs 封面}

[A Beginner’s Guide to Finding User Needs](https://urbook.fordes.de/)

---

# 重读HIG（八）

本节是重读 Human Interface Guidelines 系列连载第八期，目的为温故知新和跟进新内容。 因为篇幅原因不会一次发布太多，之前内容已整理在 [Craft 文档](https://www.craft.do/s/fH49oLBCFdJO4l)上。

## 排版（Typography）

San Francisco 和 New York 系列都有可变字体版本，并支持动态 [optical sizes](https://fonts.google.com/knowledge/choosing_type/choosing_typefaces_that_have_optical_sizes)。

如果使用自定义字体，请尽量使之回应「显示与亮度 - 文字大小」和「辅助功能 - 显示文字大小 - 粗体文本」两个设置功能。

![动态字体.png](Scenes%20Weekly%20%2367.assets/%E5%8A%A8%E6%80%81%E5%AD%97%E4%BD%93.png)

{上图：iOS 中「显示与亮度 - 文字大小」和「辅助功能 - 显示文字大小 - 粗体文本」设置}

macOS 暂不支持动态字体。

剩下部分大都是字体间距和行高参数的参考，经典奇数字号……不再多说了。本节内容几乎没有再拿出来讲的部分，但最下方的往年 WWDC 视频依然值得一看。

→ [本节出自](https://developer.apple.com/design/human-interface-guidelines/foundations/typography)

## 访问隐私数据   (Accessing private data)

HIG 建议，仅当应用明确需要使用资源或访问数据时，才弹出请求权限提示。所以避免在应用刚一启动时请求权限，除非真的需要数据和资源才能运行（比如联网权限？）。请求权限时，也建议写清楚原因。虽然都是老生常谈，但无奈糟糕的新用户引导依然很多。

![example.png](Scenes%20Weekly%20%2367.assets/example.png)

{上图：HIG 给出的三种示例，请求权限的目的模糊不清或者干脆变成一种命令，都是不友好的}

当前应用位置权限选择分为三种：允许一次、使用 App 时允许和不允许。Apple 发现除了地图应用，大部分应用的位置权限以保护用户隐私为优先考虑的话，只需选择「允许一次」就够了。但是点击允许一次后，下次开启位置权限就要去设置里面，很不方便。所以便从 iOS 15、iPadOS 15 和 watchOS 8 开始引入了 location button [1]，以方便开发者替换选择允许一次场景的位置按钮。

- 位置按钮可以自定义图标（填充或描边）、文本、圆角和文本大小（注：SF 符号也受文本大小控制）。

[1]: 位置按钮，是 SwiftUI 的说法（LocationButton），UIKit 中是 CLLocationButton。

![location.png](Scenes%20Weekly%20%2367.assets/location.png)

{上图：左边为正常位置权限弹框，右边为按下location button 后的弹框}

理想情况下，提供一个权限的上下文说明，可以帮助用户更好地理解自己的数据如何被使用。这里暂称该界面为 Pre-alert screens（预报界面）。

- 预报界面推荐使用「继续（Continue）」或「下一步（Next）」作为按钮文本，如果是「允许（Allow）」的话，会给用户一种被操纵的感觉🕹；
- 如果预报界面的按钮不会立即唤起权限弹框，则用户会被转移注意力，也会有「被操纵感」（……总之就是不好的体验）；
- 不要在预报界面上添加多余的交互；

![Pre Alert.png](Scenes%20Weekly%20%2367.assets/Pre%20Alert.png)

{上图：两个正确的权限预报界面示例}

有几种预报界面，例如包含奖励诱导开启权限、使用系统权限弹框作为图片注解说明引导等方法，不会通过 App Store 审核。

后面还有一些风控上注意的点，不再赘述。

[Accessing private data - Patterns - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/patterns/accessing-private-data)

---

# 摘录

这周看过的一些——

> 在大公司内部创业，有一点比在外面创业轻松很多，就是不用为下个月的工资发愁。但是除了这一点不同之外，其他都是一样的。要去看市场机会在哪，要去定义产品的 PMF 功能，很多决策要考虑投入产出比，要定义阶段性里程碑，要不断招聘同学进来，要关注团队的健康发展，还要不断说服上级老板认可并持续投资，这些都是一样的。

—— 玉伯 - 《[语雀的源起、定位与世界观](https://mp.weixin.qq.com/s/xd7uAsivYE1PJRfKKfeTBw)》

---

# 小事

1、意大利面食品牌百味来（Barilla）每个 Spotify 歌单长度正好对应了不同面条的烹饪时间。讨巧的营销。

![截屏2022-08-27 13.38.02.png](Scenes%20Weekly%20%2367.assets/%E6%88%AA%E5%B1%8F2022-08-27%2013.38.02.png)

{上图：煮意式细面需要 9 分钟的歌单}

[Barilla Italia](https://open.spotify.com/user/w2p1oq867ns7jele6g3lw66fk)

---

2、Neal Fun 的小游戏网站总是不会让我们失望，新上线的 Design the Next iPhone 充分发挥了 [Neal Agarwal](https://twitter.com/nealagarwal) 的整蛊天赋。

![Frame 38.png](Scenes%20Weekly%20%2367.assets/Frame%2038.png)

{上图：果式配件集合体}

除了贴 Android 会降价这种彩蛋外，有人发现其 HDRI 贴图是 Apple Park。甚至有人将自己的创作 mint 到[OpenSea](https://opensea.io/assets/ethereum/0x495f947276749ce646f68ac8c248420045cb7b5e/105194599681972540636900637341724545673537690943627690231417169880329828171777) 上……

[Design the next iPhone](https://neal.fun/design-the-next-iphone/)

---

3、时隔 20 多年，CSS 的 **:has()**伪类终于突破了性能阻碍，开始走到大众面前。在我刚接触 CSS 时，> 选择器用于匹配子元素已流行多年，但是一直没有反过来匹配父元素的选择器让我很疑惑，导致很多实现需要依靠Javascript 获取DOM 元素。:has() 的支持又扩展了 CSS 能力，而且语义通畅，支持与其他伪类、子选择器和兄弟选择器一起使用。WebKit 博客已有很多例子讲解，比如无需 JS 来实现浅色/深色模式切换🤯。

Safari 从 15.4 版本开始支持，Chromium 在 8 月末的 105 版本也会支持，Mozilla 也在推进 Firefox 兼容。下方链接建议在相应版本的浏览器中打开。

![caniuse.png](Scenes%20Weekly%20%2367.assets/caniuse.png)

{上图：Can I Use 上当前 :has() 浏览器兼容性一览 }

[Using :has() as a CSS Parent Selector and much more](https://webkit.org/blog/13096/css-has-pseudo-class/)

[来了，来了，CSS :has()伪类她来了 « 张鑫旭-鑫空间-鑫生活](https://www.zhangxinxu.com/wordpress/2022/08/css-has-pseudo-class/)

---

4、Landing Page 展示网站有不少，但是像 **Great Landing Page Copy**（后简 GLPC***）**这样专门展示文案的倒是头一次见。他们认为大多网站文案像是*”goddamn lawyer”所写（律师朋友不要介意🥶），GLPC 的目的就是展示一些易读易懂，尊敬用户的优秀网站文案。

比如下图这个售卖伏特加的网站，开场直白地告诉你 Alcoholic Vodka 的危害：对你的健康非常有害，又贵。利用了出丑效应（Pratfall Effect）来博得消费者好感。

![Vodka.png](Scenes%20Weekly%20%2367.assets/Vodka.png)

{上图：Alcoholic Vodka 案例简析}

→  回顾：[第 63 期](https://designscenes.zhubai.love/posts/2165749375996317696)提到了 [Copywriting Examples](https://designscenes.zhubai.love/posts/2165749375996317696#:~:text=4%E3%80%81-,Copywriting%20Examples,-%E6%98%AF%E4%B8%80%E4%B8%AA%E6%96%87%E6%A1%88) 也是一个展示技巧文案的网站。这边更偏向着陆页给人留下的第一印象。

[Great Landing Page Copy is a little corner of the internet to find great landing page copywriting examples.](https://greatlandingpagecopy.com/)

---

5、继续 AI Art——

[Stable Diffusion](https://github.com/CompVis/stable-diffusion) 的开源又为人工智能生成图像领域注入不少生机。DreamStudio 就是利用该引擎的网站之一，注册就送200 credits，根据不同的分辨率、生成步骤和 Cfg 比例（越高越好）制定单张图的花费。实际生成效果并不太理想，调教甚至不如 [craiyon](https://www.craiyon.com/)，与 Midjourney 也有很大的距离，我的描述（prompts）写得不够好也是很大的原因。

[DreamStudio](https://beta.dreamstudio.ai/)

另外，有人做了个 DALL·E 2 版的 Pinterest，名叫 OpenArt。搜集了大量 DALL·E 2 生成图片和对应描述，可根据风格，体裁和视角筛选。整体比较简陋，但终归有人做了这个。目前还欠缺一些版权声明。

[Discovery | OpenArt](https://openart.ai/discovery)

NLP 数据科学家 Lucy 在收到 DALL·E 2 邀请后，以一些著名的专辑封面为灵感描述，看看 DALL·E 2 能整出什么活，结果也是啼笑皆非。值得注意的话，Lucy 一直没用用到 Album 相关词汇暗示。

![Album.png](Scenes%20Weekly%20%2367.assets/Album.png)

{上图：使用 Wish You Were Here 专辑为灵感，根据描述生成的八张图片}

一些结论和以往得出的一样，比如 DALL·E 2 不擅长处理图片中加入文字，对介词不敏感。

[I recreated famous album covers with DALL-E](https://lucytalksdata.com/i-receated-famous-album-covers-with-dalle/)

---

6、Steam Deck 发布了一本手册，用于介绍 Valve、Steam 和 Steam Deck。Steam Deck 的想法源于 10 年前开发 Steam Controller，但当时硬件能力跟不上。后来 SteamOS 和 Valve Index也让 V 社积累相当的经验。读完发现其实强调的是 Steam Deck 集 V 社多年技术沉淀之大成。还夹杂着些许有趣的 Deck 品牌标识延展。

![image 40.png](Scenes%20Weekly%20%2367.assets/image%2040.png)

{上图：Steam Deck 的可爱手绘}

该手册也会在东京电玩展（TGS）上分发实体版本。

最近 Valve 着手重设计两年未更新的 [Steam 移动端](https://steamcommunity.com/games/593110/announcements/detail/3335498663100828299)也令人感到惊讶，如有机会上手体验会第一时间分享。之前对[游戏宣传图的新规](https://store.steampowered.com/news/group/4145017/view/6232436041608114694)调整也将于 9 月 1 号实施，同样是件好事。

[Publications - Valve Corporation](https://www.valvesoftware.com/en/publications)

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

![1500x500.jpeg](Scenes%20Weekly%20%2367.assets/1500x500.jpeg)

{上图：2022 科隆游戏展}

**科隆游戏展**重回线下，连展前发布会都显得比 E3 还要热闹。

以下链接均摘自 IGN 中国。

新的《[索尼克 未知边境](https://www.bilibili.com/video/BV1fd4y1w7ok)》预告比之前强上不少，但依然掩盖不了一些远景模糊、细节贫瘠的场面。鉴于之前媒体对其玩法的吐槽，依然不做期待。

[DuelSenes Edge](https://www.bilibili.com/video/BV1gT411w7JX) 作为蓝队的 「精英版」，由于双摇杆布局都在下方，便可自定义更换摇杆模块，而不仅是更换摇杆帽。我的 PS5 摇杆还没漂移，而且对Xbox 精英手柄体验并无感受到差异……索尼先继续断气吧。

自 2018 年泄露，之后跳票多次的《[霍格沃茨：遗产](https://www.bilibili.com/video/BV1mD4y1z7k6)》这次 PV 有点力不从心，对比先前的多次预告片，这次反而让人有点「食欲下降」。

《[木卫四协议](https://www.bilibili.com/video/BV1xa41197Nw)》的实机预告进一步强调了自己作为《死亡空间》续作的「正统性」——高度的血腥、沉浸的叙事性UI、断肢机制。如果它没那么 horror 的话还是可以试试。

《[Lies Of P](https://www.bilibili.com/video/BV1pP411574U/?spm_id_from=333.788.recommend_more_video.-1&vd_source=d26df9da1e716a5c0a85b7e737b2c0c7)》由韩国 NEOWIZ GAMES《神佑释放》的那个组制作，虽然满屏透着一股[血源](https://en.wikipedia.org/wiki/Bloodborne)味，但是魂系游戏只从视频看尚不能盖棺定论。

死亡岛系列一直把PV做的很有调性，这次时隔多年的《[死亡岛2](https://www.bilibili.com/video/BV1zD4y1z7AP)》又有了新的CG 预告，奈何多次更换制作组，玩家在如今又有多部射击丧尸类游戏的灌输，《死亡岛2》能否打开一条新的路？

这次 *[Forspoken](https://www.bilibili.com/video/BV1rB4y1V7Rh)* 实机预告加入了一些新的魔法演示，最主要的是加入了起始剧情简介……总担心女主会使用某些西方价值观做出奇怪的事。夜光引擎的魔法材质依然出色，但是城镇内容看着比较空，该作大概率是快餐化作品。

我没玩过[幻想水浒传](https://zh.wikipedia.org/zh-sg/%E5%B9%BB%E6%83%B3%E6%B0%B4%E6%BB%B8%E5%82%B3%E7%B3%BB%E5%88%97)系列，所以也对现代精神续作《[百英雄传](https://www.bilibili.com/video/BV1YU4y1k7zm)》充满了期待。多角色 JRPG 「量」是基础，如果「质」有 Chrono Cross 般……那可能真是幻想了。《百英雄传》习得 HD-2D 的景深真传，将其融入到战斗中，效果非常不错。

这几年对射击游戏有很强的免疫性，即便如 [Prey](https://store.steampowered.com/app/480490/Prey/) 般优秀作品也未能完整体验下来。《原子之心》战斗预告让人重回生化奇兵那种多样战斗与场景美学的融合。如果有时间，真想和《[System Shock](https://www.bilibili.com/video/BV1Kg411D7ut)》一起体验啊。

任天堂的树屋除了有我不玩的《[斯普拉遁3](https://www.bilibili.com/video/BV1ud4y1m75H)》，居然还有Square Enix 的 *HARVESTELLA* 演示。符文工房式的内核注定这游戏走不进大众目光，加上 SE 以往高额的售价，有些堪忧……

之前 PS2 版铳墓游戏 *Gungrave: Overdose* 一言蔽之相当于鬼泣中的但丁只用黑檀木与白象牙花式射击，不用瞄准（当然）。继 [VR 版](https://store.steampowered.com/app/892210/GUNGRAVE_VR/)后续集，《[铳墓 G.O.R.E](https://www.bilibili.com/video/BV1BT411w73a)》沉默已久后公布了发售日，想尝鲜。

截至今天的预告片中（有很多我没提到），期待最高的还是 Team NINJA 的《[卧龙：苍天陨落](https://www.bilibili.com/video/BV1yG411V7LD)》。忍者组的动作底蕴太深厚，例如双剑武器在数个游戏动作模组都有差异。而且我挺喜欢他们抛弃武器自身物理属性的机制（双手重武器就一定要前摇后摇慢动作迟缓吗）。自带中文配音也正好迎合了国内的民族主义，这不大卖没道理。

→ 更多展会视频

[IGN中国的个人空间_哔哩哔哩_Bilibili](https://space.bilibili.com/652239032/search/video?keyword=Gamescom)

→ 科隆所有游戏

[Games | gamescom](https://www.gamescom.global/en/games?sorting=relevance)

---

# 映像

现实拟像放映——

![JWST_2022-07-27_Jupiter_2color-2048x1765.png](Scenes%20Weekly%20%2367.assets/JWST_2022-07-27_Jupiter_2color-2048x1765.png)

{上图：使用 F212N（橙色）和 F335M（青色）滤光片的 Webb NIRCam 合成图像}

放大后可以看到木卫五、木卫十五和木星环。

JWST 的合成照片兼具科学价值和大众科普价值，太难得了。关于如何合成这样惊艳的照片，NASA [也有介绍](https://www.nasa.gov/mediacast/gravity-assist-how-we-make-webb-and-hubble-images)。

Credit: NASA, ESA, CSA, Jupiter ERS Team; Image processing by Ricardo Hueso (UPV/EHU) and Judy Schmidt.

[Webb’s Jupiter Images Showcase Auroras, Hazes – James Webb Space Telescope](https://blogs.nasa.gov/webb/2022/08/22/webbs-jupiter-images-showcase-auroras-hazes/)

---

# 温故

[Scenes Weekly | No. 18](https://mp.weixin.qq.com/s/SrUwpBE0u3rZfzPk2tM-ew)

- MAD 团队关于 OS 风格网站制作分享
- OTF 字体特性数据库 惆怅长岑长擦擦擦擦擦擦擦擦擦擦擦擦擦擦擦擦擦擦擦擦擦
- Twitter和 Grilli Type 合作定制字体 Chirp 上线
- Normform 网格图案生成
    - 注：185 期后停止更新，之后网站也无法访问，作者把所有图案放到了 Adobe Stock 上了
- iOS 15 Safari 重设计再争议
- Oculus 的品牌更新

---

喜欢本文的话，欢迎分享、订阅。

第 66 期请[在此查看](./Scenes Weekly #66.md)。

本次封面使用了The Aesthetic Essential 字体。