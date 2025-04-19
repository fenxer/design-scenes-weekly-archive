# Scenes Weekly #66

2022-08-22

\> 设计视角下的世界——

第 65 期请在此查看。

本期出现：

- Color & Contrast 颜色指南
- 交互式语音应答系统设计
- Altar I 客制化键盘初探
- App 内嵌浏览器与隐私
- Newsletter 历史回顾
- 重读 HIG（七）
- 其他：更加现实的 Fockups、好莱坞特效行业危机、社交与第三空间

如有格式异常建议点击最上方「在浏览器中访问」。

---

上周在 [DEX周刊 #152](https://dex.zhubai.love/posts/2170932605460406272) 看到关于某位热衷于 Twitter Thread 内容的创作者，暂且不展开讨论——以自己没有机翻行为回复对方提出的「机翻味」——这种无效反驳。Thread 功能上线已有近 5 年，像 [Julie Zhuo](https://twitter.com/joulee) 等大V便是其重度用户。虽然 Thread 形式上远不如文章，但有很强的传播性。Twitter 很多用户已经厌倦了这种**说教味**内容出现在信息流——特别是当你的内容没什么意义的时候。

我没有称该事件为「瓜」的原因是，这也促使了对本通讯内容的反思。特别是新增的重读 HIG 一栏，由于原规范就有多处使用祈使句的地方，加上本来是类似阅读笔记一样的风格，在没有特意转变表达方式时就会很担心说教味的浓度。我只能简单地尽可能去掉主语，或者把「你」改成「我们」这样。如果本通讯内容对你有所不适，请直接回复此邮件告诉我😇。之后也是。

然后，欢迎上周的新订阅者。感谢所有订阅者的支持。

---

# 杂事

1、[Nate Baldwin](https://natebaldw.in/) 的 Color & Contrast 网站详细地介绍了界面上的颜色学。以视觉生理为开端，从色觉到错视原理、从视障到光学现象、从颜色学到可视化，每个条目都有说明如何界面设计，可交互的控件和统一的插图带来了绝佳的综合指南体验。

![可见光.png](Scenes%20Weekly%20%2366.assets/%E5%8F%AF%E8%A7%81%E5%85%89.png)

{上图：可见光中三原色波长示意}

→ 网站

[Color & Contrast](https://colorandcontrast.com/#/)

---

2、好久没有提起 Nielsen Norman Group，这次他们介绍了平时几乎接触不到的 Phone-Tree Systems 设计，也就是打电信运营商客服时常听到的交互式语音应答系统（IVR）。

NN/g 的文章一如既往结构清晰，首先列举了人们通过电话联系客服的四种类型原因：

- 在线客服没有达到预期或没有解决问题，转而求助语音客服；
- 遇到的障碍阻止他们正常进行任务；
- 无法自己整理清楚混乱的信息；
- 单方面认为在线任务太过于复杂打字讲述不明白，更想和真人交谈；

感觉这四种原因差的不是太多……但是 Phone-Tree 系统 系统的难处很明显：

- 发达的在线服务使 Phone-Tree 逐渐没落，但是一旦在线服务出现问题，便需要转至电话服务，一些体验尚未优化的电话客服则会又引导用户转至在线服务解决；
- 有时用户只想和真人客服交谈，却需要通过重重自动应答。企业则想利用自动应答减少真人客服成本；
- 用户呼叫电话客服通常说明已经「走投无路」——他们本可以转为使用另一个相似服务，但是没有；此时 Phone-Tree 设计体验不佳的话，会更令人困扰；
- 电话客服依赖听说能力；

![irs-phone-tree7.png](Scenes%20Weekly%20%2366.assets/irs-phone-tree7.png)

{上图：美国国税局的 Phone-Tree 路径结构，纵向最深有10个层级}

NN/g 为此对 12 个大企业的 Phone-Tree 系统进行了评审，并且给出了 16 条建议：

- 涉及到多语言业务解除的企业，应在 Phone-Tree 先提供语言选项；
- 帮助呼叫者记住信息，比如事先提示对方准备纸笔、慢语速重复或选择接受相关信息短信等方法；
- 仅向呼叫者提供有帮助信息的网页，而不是企业首页。如遇到很长的网址，也要注意上一条建议；
- 使用相同的按键名称，统一按键控制。比如 # 号键，在美国常读作 pound，在英国却常用 hash 表示，不一致的叫法会让人分心。业内常见交互模式有：
    - 使用 # 号键撤销操作，或者用来提交输入信息；
    - 使用 * 号键复读当前菜单选项；
    - 呼叫者没有做出选择时，自动复读当前菜单选项；
    - 如果呼叫者让当前菜单复读了三遍，则直接连接到人工客服（美国万豪酒店会直接挂掉……）；
    - 菜单选择以 1 键开头；
    - 菜单的顺序由使用频率决定，越往后越不常用；
    - 允许呼叫者直接按 0 连接人工客服；
- 始终允许呼叫者撤销操作，而不是从头重新选择一遍；
- 避免同一层级过多的菜单选择，尽量区分开每个菜单的文案用语；
- 如果一开始有呼叫询问环节（用自然语言描述遇到的问题），可以给出一个跳过的选项；
- 企业没有7 x 24 小时电话应答时，应在录音里提示：
    - 营业时间；
    - 引导至解决常见问题的页面；
    - 某些行业里，还会留下紧急联系人；
- 简单点，如不必要不加多余的宣传广告等冗长的开头信息；
- 向呼叫者提供简单的反馈，比如按键音、按键播报等；
- 给呼叫者更多点时间，一般用于临时查找信息。希尔顿酒店电话就允许呼叫者回复”*More time*”来延长时间，此时可以挂起呼叫并专心寻找号码，找到后可以按 1 回到呼叫中；
- 尝试举例说明以帮助呼叫者快速找到信息；
- 每个菜单选择播报顺序可以是，先说菜单信息，再说对应的数字按键。这个小细节可以让呼叫者只需记得自己相关情况的数字；
- 录制真人讲话而不是使用合成的机器语音；
- 等待人工客服时，以适当频率提供定期更新的信息；

虽然上述建议对象是 Phone-Tree 系统，但原理上依然离不开基本的交互法则，对界面设计也有一定的启发性。

→ 查看原文更多举例

[The UX of Phone-Tree Systems: 16 Usability Guidelines](https://www.nngroup.com/articles/phone-tree-guidelines/)

---

3、精良的 Mockups 是设计包装的重要环节，但功能主义（functionalism）的凝视者早就看这些图片不爽了——

> These f*cked-up mockups show your design in a realistic way. Because eventually, people will be checking their phones when they are taking a sh*t rather than looking at an expensive iPhone floating through space."

所以 Wytze Hoogslag 设计了一系列比较现实的 mockups，称之为 Fockups。意在打破传统 mockup 中的美好幻想，回归生活中的种种偶然和差错。它的画风是这样的：

![Fockups_phone.png](Scenes%20Weekly%20%2366.assets/Fockups_phone.png)

{上图：男人厕所玩手机}

![Fockups_Businesscard_Asize.png](Scenes%20Weekly%20%2366.assets/Fockups_Businesscard_Asize.png)

{上图：埋汰的地面上一张折痕严重的名片}

该死，这种心动的感觉……于是立马买来收藏，并开始盼望着以后能用到。

→ 更多款式

[Fockups – F*cked up mockups](https://fockups.com/)

---

# 重读 HIG（七）

本节是重读 Human Interface Guidelines 系列连载第七期，目的为温故知新和跟进新内容。 因为篇幅原因不会一次发布太多，之后会专门整理。

这周终于写到了 HIG 新内容之一，RTL。

## Right to left

- 系统组件默认带有 RTL 转换，调用后不需要手动调整；
- 文本段落对齐，HIG 建议遵循不同语言的阅读顺序习惯。例如下图英阿混排时，单独排版提高易读性；

![RTL-1.png](Scenes%20Weekly%20%2366.assets/RTL-1.png)

{上图：RTL 书写系统中插入 LTR 文本的正确排版方式}

- 但是当文本元素以列表形式表现时，为了确保一致的浏览体验，建议统一遵循 RTL；

![RTL-2.png](Scenes%20Weekly%20%2366.assets/RTL-2.png)

{上图：RTL 列表中插入 LTR 内容时的正确排版方式}

- 不同的 RTL 语言会使用不同的数字体系，例如：
    - 希伯来文使用西方阿拉伯数字（0123…）；
    - 阿拉伯文使用东方阿拉伯数字（٠١٢٣…）；
        - 东方阿拉伯数字又分为[三种](https://en.wikipedia.org/wiki/Hindu%E2%80%93Arabic_numeral_system)：标准阿拉伯语系、波斯语系和乌尔都语体系；
    - 不同数字体系使用因国家和地区而异；
- 不要颠倒一串数字的内部顺序；
- 一些控件变换为 RLT 顺序后，数字也应随之变换。HIG 举例了评分系统：

![截屏2022-08-15 16.50.16.png](Scenes%20Weekly%20%2366.assets/%E6%88%AA%E5%B1%8F2022-08-15%2016.50.16.png)

{上图：五星评分控件在拉丁文、阿拉伯文（东/西方阿拉伯数字）和希伯来文中的顺序}

- 同时控件顺序的改变也表明，我们习以为常从左向右滑动的顺序，与平时阅读习惯有很大关联；

![RTL-control.png](Scenes%20Weekly%20%2366.assets/RTL-control.png)

{上图：iOS 图书应用中一些控件的 RTL 变换}

- 但是当某控件在指示具体方向时（上下左右），该控件本身不受 RTL / LTR 影响。而上图的返回箭头（chevron），目的是指向屏幕外方向，所以才会指示方向和位置一起翻转；
    - 同理，一些图片、图标和艺术作品，翻转后如果改变了本身含义，便不必翻转。例如地球图标和蒙娜丽莎；
- 一些 RTL 文字相比同字号大写拉丁字母显得比较小，HIG 建议可以将其增加 2pt（often works well）或其他合适数值匹配；
- 一些界面图标的 RTL 适配在[图标](https://developer.apple.com/design/human-interface-guidelines/foundations/icons)一节中已提到，在本节中有了更多 RTL 图标示例，推荐到原文观看；

→ 本节出自

[Right to left - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/right-to-left)

## SF 符号（SF Symbols）

- SF Symbols 最大的特色是与 San Francisco 字体系列的高度集成，大小和粗细与文本对齐。但也继承了 iOS 字体排版薄弱的一面；
- SF Symbols 图标根据 icon 图层层级命名。比如 cloud.sun.rain.fill 图标即分为三层：
    - 第一层 cloud，第二层 sun，第三层 rain；
    - 层级与 Z 轴关联。换句话说，第一层是 sun 第二层 cloud 的话，太阳就会遮住云彩；
    - 图标是填充类型，最后加上 .fill；

![rain.png](Scenes%20Weekly%20%2366.assets/rain.png)

{上图：cloud.sun.rain.fill 多云转雨 (?) 图标的三个图层级解析}

- 每个层级可单独上色，可以在 SF Symbols 应用中调试；
- 我们也可以使用 SF Symbols 应用自定义图标，但是极其麻烦（**这节可以读到这里跳过了**）。是不是 Apple 也知道自定义图标麻烦，所以自己每年都猛增图标个数😇；
    - 首先 SF Symbols 不像 [iconfont](https://www.iconfont.cn/) 那样提供通用的模板——事实上它确实有模板，但是需要单独导出（选中图标 - 文件 - 导出模板[⌘E]）；
    - 导出的模板非常复杂，建议模板设置选择「可变」导出，这样只需要设计其中三个图标而不是所有 27 个😅；

![custom.heart.fill.png](Scenes%20Weekly%20%2366.assets/custom.heart.fill.png)

{上图：SF Symbols 的自定义图标模板}

- 该模板 HIG 推荐使用 Sketch 和 Adobe Illustrator 编辑，无法使用 Figma，因为导出 SVG 时会破坏所有其中分组文件夹，SF Symbols 正是依靠其中各个文件夹来识别变体；
- 将改动后的模板拖到 SF Symbols 中，遵循上述图标命名法更改图标名称，然后在 Layers 里定义层级（最多三层），如下图：

![custom.png](Scenes%20Weekly%20%2366.assets/custom.png)

{上图：SF Symbols 4 中定义图标的图层}

- 配置完毕后选择「文件 - 导出符号（⇧⌘E）」，给开发扔进 Xcode 里使用……

→ 本节出自

[SF Symbols - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/sf-symbols)

→ 自定义符号（视频）

[Create custom symbols - WWDC21 - Videos - Apple Developer](https://developer.apple.com/videos/play/wwdc2021/10250/)

→ 自定义符号（开发文档）

[Apple Developer Documentation](https://developer.apple.com/documentation/uikit/uiimage/creating_custom_symbol_images_for_your_app/)

---

# 摘录

这周看过的一些——

> 像米开朗基罗一样，伯尔尼尼精心研究，细心描画了梵蒂冈的古代雕像收藏品，从典雅的《瞭望塔中的阿波罗》直到传世古典作品中最狂烈、最有戏剧性的群雕：拉奥孔及其两个儿子与大蛇搏斗的雕像。这些雕像反映出古人对解剖有惊人的知识，了解身体的运动，也反映出他们在构图时的多样性和表现皮肤、毛发、鸟羽、兽皮、人物穿着时的自然主义手法。他还在童年时代就被这些东西迷住了，当时他唯一的愿望就是要和它们一比高低。这一点可以从他传世的最早作品之一《母羊阿玛尔忒亚和婴儿时期的朱庇特及牧神》中看得很清楚，据说这件作品是他刻着玩的，但它表现得如此逼真，人们长期以来以为是古代的作品。

> 但伯尔尼尼并不止于与古代雕刻家相媲美，正像阿尼巴·卡拉奇有感于古老的神话而画出新的、活生生的自然场面，伯尔尼尼则试图用**戏剧性的、有生命的**塑像来再现神话故事。

——《剑桥艺术史：17世纪艺术》

---

# 小事

1、好莱坞特效行业苦痛的打工现状：

- 复仇者联盟里黑寡妇的一头红发，是让斯嘉丽·约翰逊先带上假发后，整个特效团队花了两周时间一根根处理的；
- 片场没做好的事，都留给了后期特效团队；
- 作品发布日期不会因后期制作而多考虑；
- 连续几天工作超过 14 小时；
- 给老哈里森·福特修下巴；
- 每天收到的原片时间都很少低于 240 分钟，甚至行尸走肉一集有 7 小时；
- 渲染时期就是待命阶段，刷 Twitter 都能刷到厌烦；
- 时间也常常浪费在修复随机背景颜色上的镜头，这些颜色可能是摄像师（DP）指定的；
- 作为 VFX 工作者不允许以个人名义展示自己的作品；
- ……

评论里有人提到了，当年获得奥斯卡最佳视觉效果奖项的《少年 Pi 的奇幻漂流》，其背后的工作室 Rhythm & Hues Studios 当年便申请了破产保护，理由为行业艰难，利润微薄加上 2012 年并没有接到太多工作。

→  原文

[Inside Hollywood's Visual Effects Crisis | Defector](https://defector.com/inside-hollywoods-visual-effects-crisis/)

---

2、笑盐LaughTale 的 ***The Great Good Place*** 读书笔记以「第三空间」的角度剖析了纯粹的社交。在这个平等空间里，没有互联网熟人和陌生人社交的清晰界限，作者在试着以现实的社交规则去映照互联网社区的模样。

![book.jpeg](Scenes%20Weekly%20%2366.assets/book.jpeg)

{上图：*The Great Good Place 书封面*}

→ 原文

[可能是最好的互联网社区入门读物 The Great Good Place](https://mp.weixin.qq.com/s/9AT1acNGsSQjjMMdHa31jQ)

---

3、**Electronic Materials Office** 发布了一款 Altar I 薄款客制化键盘。

- 可回收铝和PBT 外壳；
- 凯华的巧克力v1矮轴（Kailh Choc Low Profile v1）；
- ZMK 固件；
- 500 mAh 电池（太小了吧）；
- 重 635 克；
- 蓝牙（5.0, BLE）连接最多两台设备；
- 凹陷和凸起并存的一套键帽；
- 特色旋钮；

![layouts.jpeg](Scenes%20Weekly%20%2366.assets/layouts.jpeg)

{上图：Altar I 美式布局}

最令人（可能只有设计师群体）眼前一亮的是，它的 logo 采用了 Display Type Foundry 的 [Tobias](https://displaay.net/typeface/tobias/) 字体，键盘铭刻采用了 Grilli Type 的 [GT Flexa](https://www.grillitype.com/typeface/gt-flexa) 字体。整体看上去非常精致，像是新拟物风格（Neuomorphism）的实体化。

但是——但是，这把键盘还有很多疑问，比如：

- 字母区紧凑的布局不熟悉的人误触是肯定的了，但是底部凸起的 ⌥ ⌘ 以及空格，在按上方 ZXC一排时是否更容易误触呢，说到底这种凹凸分割布局的手感还有待观望；
- 无论是美式还是欧式布局，最右边放 logo 处留白而不是放置 PageUp/Down、Home 或 End 等功能按键；
- 按键清理貌似更难了；
- 脚垫还不清楚什么结构，或者是没有脚垫？
- 旋转按钮太高了，携带时肯定会不方便（参考手柄摇杆不带外包装的话有多危险）。如果旋钮可拆卸，希望键盘有地方收纳；

![hero-2.jpeg](Scenes%20Weekly%20%2366.assets/hero-2.jpeg)

{上图：Altar I 旋钮部位特写}

Electronic Materials Office 官网也做的很棒，但目前透露信息很有限。

→ 官网

[Electronic Materials Office®](https://electronicmaterialsoffice.com/)

---

4、Felix Krause（[第52期](https://designscenes.zhubai.love/posts/2132756592087695360#:~:text=7%E3%80%81-,Felix%20Krause,-%E5%9C%A8%E8%BF%87%E5%8E%BB%E4%B8%89%E5%B9%B4)也提到过老哥）做了一个 [InAppBrowser.com](http://InAppBrowser.com) 工具，用于检测应用内嵌浏览器是否有将 JavaScript 代码注入第三方网站。结果在 TikTok 中发现了严重的劫持风险——当你在 iOS TikTok 中打开任何链接时，TikTok 会监测你的键盘输入以及点击行文。TikTok 承认了这些代码的存在，但是「我们没有使用它，仅用于调试和性能就监测」😅。

然后我随手测了几个常用的国内移动应用，结果在飞书和支付宝里也发现了监测行为……

![inApp.png](Scenes%20Weekly%20%2366.assets/inApp.png)

{上图：飞书内嵌浏览器会监测你在第三方网站的输入和点击行为，支付宝则是监测点击和文本框对焦行为}

当然，像是支付宝检测输入框焦点，理想情况可能真是在做风控。值得一提的是，在 iOS 中开启锁定模式可屏蔽这些监测。

→ 原文

[https://krausefx.com/blog/announcing-inappbrowsercom-see-what-javascript-commands-get-executed-in-an-in-app-browser](https://krausefx.com/blog/announcing-inappbrowsercom-see-what-javascript-commands-get-executed-in-an-in-app-browser)

---

5、Newsletter 的热潮似乎已经退去，我们都很欢迎那些欢愉炒作后的坚持留下来认真写作的人，SubStack 的财富神话在现实数据面前不再诱人，Bulletin（Meta 旗下的）停止了进一步运营招募创作者，Revue 品牌被并入 [@Twitter Write](https://twitter.com/TwitterWrite) 一起风雨飘摇。很多独立记者下场后发现订阅收入并不如自己本职薪资高而又另寻出路，而在另一种环境的国内，更多的是对无止境扩张的信息聚合以及推荐算法牢笼的反抗，newsletter 填补了到个人之间交流的空白。

Newsletter 最早可追溯至罗马帝国的[私人信件](https://www.worldhistory.org/article/1442/letters--post-in-the-ancient-world/#:~:text=also%20wrote%20handbooks%20with%20sample%20letters%20and%20academic%20commentaries)。文艺复兴时期，奥格斯堡贵族商人富尔格家族（Fugger family）依靠各地通讯员提供财务数据和政治评论（还有一些军事、犯罪、忏悔和庆祝活动等主题，[详见](https://fuggerzeitungen.univie.ac.at/en/about-fugger-newsletters)），虽然这些评论基本持有无异的（宗教）立场，并非客观讨论时事。时到如今，大型时事通讯之一 Morning Brew 也是金融和商业为主题（截至今年 3 月份有超过 400 万订阅者，详见[第49期](https://designscenes.zhubai.love/posts/2125143039055626240#:~:text=4%E3%80%81CNBC%20%E5%AF%B9-,Morning%20Brew,-%E7%9A%84%E4%B8%80%E7%AF%87%E6%8A%A5%E9%81%93)）。 

![Fugger.png](Scenes%20Weekly%20%2366.assets/Fugger.png)

{上图：News and rumor in Renaissance Europe; the Fugger newsletters 一书封面}

几百年过去，1920 年前美联社记者 Willard Monroe Kiplinger 推出了金融（个人理财）为主题的 newsletter，这是第一封现代意义上的 newsletter，并推动了 20 世纪 newsletter 的发展。而让 newsletter 蓬勃发展挺近 21 世纪的是 Howard Penn Hudson。这位传统纸媒记者经营着很多细分领域的出版，涉及到军事、室内植物打理、能源政策、野外求生、市井八卦等等，每次不超过 16 页，没有封面头版和广告，订阅制。

后来他收购了一家 The Newsletter on Newsletters 通讯，负责教育他人怎么写 newsletter，还创办了全国性质的通讯出版协会（Specialized Information Publishers Association 前身，后被 Software & Information Industry Association 收购）。Hudson 认为许多学生写作时缺乏两个重要的因素：

- 向他人传达信息的前提是可理解性；
- 写作当做爱好，一种生活习惯；

![Content.png](Scenes%20Weekly%20%2366.assets/Content.png)

{上图：1982 年 Hudson 所著 Publishing newsletters 一书目录}

除此之外，Hudson 还有一些现在看起来比较有趣的观点：

- 订阅是规则，不容异议；
- 华盛顿是 newsletter 的摇篮，政府一手信息，记者集中，「在政府学会用英语写作之前，我们是安全的」；
- 细分领域（niche）是一切，必须把目标缩小；
- 简洁，一寸纸张一寸金。数字时代也需要这种写作能力；
- 广告宣传很痛苦。虽然使用邮件宣传不会像电话营销那样直接，但也会激怒一些人。Hudson 在书中还提到了租用邮件列表的想法，成本每千人 45 美元，放到现在就是 spam；
- Newsletter 很容易使人倦怠，一个要做的事情太多了——确实；
- 施乐的打印机对 newsletter 是一个很大的风险，有人会用此机器分发盗版复印件；
- Newsletter 的订阅者更容易接受其创作者额外的交易服务，所谓粉丝经济；

→ 原文

[What Newsletter Authors Can Learn from the Print Newsletter Era](https://tedium.co/2022/08/10/pre-digital-newsletter-history/)

---

我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 0 个订阅。

→ [详见](https://fenx.work/design/newsletter) *(notion.com)*

→ [封面存档](https://www.figma.com/community/file/1139404827019734932) *(figma.com)*

→ [关于本通讯](https://designscenes.zhubai.love/posts/2165376854788718592) *(zhubai.love)*

---

# 劳逸

![AI2.png](Scenes%20Weekly%20%2366.assets/AI2.png)

{上图：AI：梦境档案 涅槃肇始}

距离[AI：梦境档案](https://store.steampowered.com/app/948740/AI_The_Somnium_Files/)第一部发售已有近三年，第一部给了我很多惊喜，特别是临近结局前我还在思考怎么把故事圆回来时，剧情居然流畅地接上了，导致拉高了对第二部的期待。作为一款轻解密式推理游戏，诡计显得有些僵硬，不够融入（而且是制作人打越钢太郎用过的桥段），连时不时出现的黄段子也没有第一部男主讲的有意思。

在破案侦查环节增加了大量新玩法，但过多的 QTE 机制也让我流汗。第一部玩起来有很多轻松感（以至于拿了 100% 成就），这作倒是没有那么多轻松的地方了。惊喜之处是，在里面藏了一个[极限脱出3](https://store.steampowered.com/app/311240/Zero_Escape_Zero_Time_Dilemma/)的小彩蛋。

虽然感觉本作没有太吸引我的点，但打越老师的作品终究是玩一部少一部，推荐先从第一部玩玩。

→ [游戏获取](https://store.steampowered.com/app/948740/AI_The_Somnium_Files/)（第一部）

→ [游戏获取](https://store.steampowered.com/app/1449200/_AI/)（第二部）

---

# 映像

现实拟像放映——

![FZ5EA6zUIAAb1w2.jpeg](Scenes%20Weekly%20%2366.assets/FZ5EA6zUIAAb1w2.jpeg)

{上图：Figma Alpha 测试阶段收到的反馈被做成了笔记本封面}

Dylan Field 晒出的 Beta notebook

→ [推文](https://twitter.com/zoink/status/1557787837973508097)

[登录 Twitter，关注Dylan Field](https://twitter.com/zoink/status/1557787837973508097)

---

# 温故

[Scenes Weekly | No. 17](https://mp.weixin.qq.com/s/Pg3Yc7iopK8hbHJ9TcWG3A)

- 关于 to-do 应用的一些思考
- I Love Typography新栏目 ASK ILT
- 苹果线上商店更新
- Font Awesome 使用 Figma 制作图标
- Apple CSAM 评论和原理
- 网页弹窗杂谈
- Stack Overflow 公了2021 年开发者调查
- 从电子垃圾场回收的 AirPower 原型
- macOS 扫雷与蜘蛛纸牌

---

喜欢本文的话，欢迎分享、订阅。

第 65 期请[在此查看](https://designscenes.zhubai.love/posts/2170801615631011840)。

本次封面使用了 Creme Pastry 字体。