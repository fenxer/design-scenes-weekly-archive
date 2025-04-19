# Scenes Weekly #63

2022-08-01

\> 设计视角下的世界——

第 62 期请[在此查看。](./Scenes Weekly #62.md)

本期出现：

- Figma 根据背景自动变换插入文字颜色
- Anthony Burrill 的灵感收集档案
- Warp 界面字体渲染优化过程
- 重读 HIG（四）
- Wikipedia 背后的偏见
- Wikipedia 如何影响司法行为
- 其他：文案示例 Copywriting Examples、Tiimo 付费界面、This Image Does Not Exist 测验、Emoji Kitchen、One More Try 实验短片

如有格式异常建议点击最上方「在浏览器中访问」。

---

如何给一个每周通讯不写 About 页面找借口——

- 本通讯对内容结构的需求是一看便知，不需要介绍；
- 而且大部分人对陌生人的过往也不感兴趣；
- 另外与其发布一篇文章，不如在产品上加入 About 页面；
- ……

借口找完了，还是要写上。

→ [关于 Design Scenes Weekly](./关于 Design Scenes Weekly.md)

最后，欢迎上周的新订阅者们，感谢所有订阅者的支持。

---

# 杂事

1、Emma Bostian 发现了 Figma 一个小贴士，现在的 Figma 会根据背景和对比度，自动判断插入的上方文字该用白色还是黑色。

![1670062321069.gif](Scenes%20Weekly%20%2363.assets/1670062321069.gif)

{上图：Bostian 在三种饱和度紫色上测试文字颜色}

自己试了下，如果是只处于 background 上的矩形就不会识别，矩形必须在 frame 中才可以触发。另外直接在 background 上插入文字也可以判断。下方回复中有人贴出了类似代码实现原理：

```cs
Color ContrastColor(Color color){  
int d = 0;

// Counting the perceptive luminance - human eye favors green color...  
double luminance = (0.299 * color.R + 0.587 * color.G + 0.114 * color.B)/255;

if (luminance > 0.5)  
d = 0; // bright colors - black font  
else  
d = 255; // dark colors - white font

return  Color.FromArgb(d, d, d);

}

```

大意是提取出 RGB 色值，计算 R * 0.299 + G * 0.587 + B * 0.114 的和值除以 255，得到的值：

- 大于 0.5，则赋予上方文字黑色；
- 否则赋予上方文字白色；

→ 原推

[登录 Twitter，关注Emma Bostian](https://twitter.com/EmmaBostian/status/1550056313291522054)

---

2、平面艺术家 [Anthony Burrill](https://anthonyburrill.com/) 与设计师 [Neal Fletcher](http://www.cliff.studio/) 和 [Richard Nicholls](https://designedbyrich.co.uk/) 合作推出了一个在线档案。该网站搜集了 Burrill 平时的创作灵感等琐碎设计，类型包括符号、箭头、图标、插画、字母、数字、图案、海报、印章和贴纸等等。所有作品都是黑白色调，Burrill 觉得 “so strong”、“just incredible”。

![1670062324122.jpeg](Scenes%20Weekly%20%2363.assets/1670062324122.jpeg)

{上图：Burrill 的在线档案部分截图}

Burrill 在推动跨领域的凸版印刷领域闻名，他的作品善用粗犷的笔画来表现文字的重量，在这个档案网站里可见一斑。

→ 网站

[Anthony Burrill](https://anthonyburrill.xyz/)

---

3、开箱即用的友好型终端 Warp 最近在博客中分享了他们的界面字体渲染方法。由于 Warp [使用 GPU 渲染界面](https://www.warp.dev/blog/how-to-draw-styled-rectangles-using-the-gpu-and-metal#why-render-on-the-gpu)，所以字体显示方面除了依赖系统库（Core Text、DirectWrite 等），也要事必躬亲。

文章先从渲染文本的两个主要部分讲起：

- Shapeing（成形）：根据 Unicode 标准将文本一对一并在正确位置显示出来；
- Rasterization（栅格化）：将矢量字体转换为基于像素的位图（GPU 先天理解不了矢量）；

### Advance Width

Advance width 在排版中指的是两个字母在 X 轴（可能是 baseline）或 Y 轴上各自 origin 点的距离。

![1670062325651.png](Scenes%20Weekly%20%2363.assets/1670062325651.png)

{上图：小写字母 a 和 f 的 width 和 advance width 属性}

如上图，红点即为 origin 点。小写字母 a 中，width 小于 advance width；小写字母 f 中，width 大于 advance width。这影响到字体排版另一更宏观的指标，kerning。（关于 advance width 详细可查看 [FreeType Glyph Conventions](https://freetype.org/freetype2/docs/glyphs/glyphs-3.html) 中的说明。）

![1670062328125.png](Scenes%20Weekly%20%2363.assets/1670062328125.png)

{上图：Glyphs 官方文档里 Kerning 一章使用大写字母 V A N D 演示}

提到 kerning 已经不再陌生，如上图 V 和 A 字偶间距的调整，使文本的负空间更和谐，看起来是 VAND 而不是 V AND。

### Rasterization

栅格化是这篇文章最有意思的一段，如下图所示。

![1670062330390.png](Scenes%20Weekly%20%2363.assets/1670062330390.png)

{上图：两种栅格化}

首先矢量边缘包围了那哪些像素中心点，哪些就会「被显示」，如上图左 1 和左 2 网格。但是这样显示出来的三角形斜边很不规整。所以有了右边的解决方法「抗锯齿」：把像素从单一采样点提升为 4 个采样点，根据包围的采样点数量不同，来显示不同饱和度的色值，如上图右 1 和右 2。这样随着采样点的提升，边缘也变得愈加平滑，渲染的性能消耗也会随之提升。

![1670062331673.gif](Scenes%20Weekly%20%2363.assets/1670062331673.gif)

{上图：16 采样点（/超采样）的 16 种灰度像素颜色}

在 LCD 或 OLED 上则是现在最常用的[亚像素渲染](https://en.Wikipedia.org/wiki/Subpixel_rendering)（subpixel rendering），对 R G B 分别采样确定各自数值，并调整至不会影响文本本身颜色。

后面内容是 Warp 讲述如何加速文本渲染，并避免文本模糊和间距不当。开发相关的内容有些超纲，有兴趣可查看原文。

→ 原文

[Adventures in Text Rendering: Kerning and Glyph Atlases](https://www.warp.dev/blog/adventures-text-rendering-kerning-glyph-atlases)

---

4、Copywriting Examples 是一个文案搜集网站，展示一些营销时的文案小贴士。他还有一个 Just Copywriting Tips 的 Twitter 账号，带有对比。比如下图建议使用转喻技巧——

![1670062333735.jpeg](Scenes%20Weekly%20%2363.assets/1670062333735.jpeg)

{上图：Stop wiping with unrecyclable toilet paper 替换为 Stop wiping with trees，1,000 songs in your media player 替换为 1,000 songs in your pocket，Go to work with an egg for breakfast 替换为 Go to work on an egg}

→ 网站

[Copywriting Examples - The world's best copy. In one place.](https://marketingexamples.com/inspiration)

---

5、我在 Screenlane 上翻到 Tiimo 这个计时应用，它的试用界面有些熟悉。正是[第 35 期](https://designscenes.zhubai.love/posts/2084557610719649792#:~:text=%E5%88%86%E4%BA%AB%E4%BA%86%E4%B8%80%E7%BB%84-,Blinkist,-%E7%9A%84%20A/B) Growth Design 分享的一个设计案例。

![1670062334978.png](Scenes%20Weekly%20%2363.assets/1670062334978.png)

{上图：左边是 Tiimo 试用付费的界面，右边是 Growth Design 分享的 Blink 案例}

巧合的是连 7-day free trial 的文案都一样😂，倒也不是挂出来责备哪方，而且也无从考据先来后到，但最终优秀的体验都会授益于用户。

→ 查看 Tiimo 其他界面

[Tiimo iOS app screenshots](https://screenlane.com/post/ios/tiimo/)

---

# 重读 HIG（四）

本节是重读 Human Interface Guidelines 系列连载第四期，目的为温故知新和跟进新内容。 因为篇幅原因不会一次发布太多，之后会专门整理。

## 图片

- 放大倍数是所有 UI 的入门课，@1x、@2x 和 @3x。HIG 鼓励使用 @1x 设计，在这个几乎达成共识的问题上，再坚持 @2x 没有意义；
- 每张图片建议都封装颜色配置文件，一般都在用 sRGB；
- 这节还详细介绍了 tvOS 带有视差效果的分层图像；

→ 本节出自

[Images - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/images)

## 包容性

- 包容性设计要求尊重每个人的立场观点，这些观点又都来源于：
    - 年龄
    - 性别和性别身份
    - 种族和民族
    - 性取向
    - 形体属性
    - 认知属性
    - 永久、暂时和情境式障碍 [1]
    - 语言和文化
    - 宗教
    - 教育
    - 政治或哲学主张
    - 社交和经济背景
- 文案上使用 you 或 your 已经挺好的了，使用 users 或 the user 会让人感到疏远）。注意 we 或 our 使用上一般指代开发的应用或背后公司就好，否则会带有居高临下的说教味道；
    - 个人看法，在中文语境包括在本通讯中，「用户」一词其实是被标签化的结果。主语是「人们」的时候，是在叙述大环境背景下的一般人。而「用户」则指代被抽象化的人群，这个人群以第三方视角描述时，带有特定的含义。HIG 这里根据上下文，说的仅是双方对话时的场景；
- 避免使用专业术语，语句尽量通俗易懂，但要注意一些幽默文案的尺度和角度；
- 代表一般人的信息时，尽量使用无性别图像表达，比如下面代表人的图标：

![1670062341311.png](Scenes%20Weekly%20%2363.assets/1670062341311.png)

{上图：从左到右图标为，圆形裁剪人像、三人群组、挥手的全身人像}

- 大多数应用不需要知道用户性别，否则只会沦为刻板印象驱动的产品；
- 提到刻板印象，除了「男医生和女护士」这种性别与职业的关联，在一些身份验证安全问题上也需注意提问内容。比如：
    - 你大学里最喜欢的科目是什么？
    - 你的第一辆车是哪个品牌的？
- 显然并不是每个人都有过大学生涯和自己的车，提问的范围可以更宽广和普遍一些；

→ 本节出自

[Inclusion - Foundations - Human Interface Guidelines - Design - Apple Developer](https://developer.apple.com/design/human-interface-guidelines/foundations/inclusion)

[1]：情境式障碍，比如冬天戴口罩，视力 1.0 的眼睛被眼镜上浓厚的雾气笼罩而看不清路和事物。

---

# 摘录

这周看过的一些——

> ​至于肩负 “沟通桥梁” 重任的专业红娘，通通都是作假包装出来的人设。 财经自媒体 “冷水财经” 曾分析，这些红娘每个人都配有单独的工作微信，头像美丽大方，简介清一色写着“婚姻家庭咨询师、国家二级心理咨询师、已婚已育、家庭幸福美满，匹配率 80%-90%”。

> 实际上，这些信息都是一键复制。 而这些专业红娘之所以能拿捏用户，是因为他们都经过专业的销售话术培训，利用 “夸、堵、戳、挖” 四个手法逐渐推进，引导会员到店咨询。

1. > 夸，业内用语 PMP，就是拍马屁的拼音缩写； 2. 堵，堵出路，让会员觉得很难靠自己找到合适的人选； 3. 戳，戳痛处，制造焦虑提高用户找对象的迫切度； 4. 挖，挖清楚用户的购买力，因为最终卖给用户的套餐是一万八还是六万八，看的不是用户的需求，而是用户口袋里的钱；

—— 王中中 - 世纪佳缘，可真 “刑” 啊

[世纪佳缘，可真“刑”啊](https://mp.weixin.qq.com/s/pArXVD16uKnhl9rHCtv29A)

---

# 小事

1、古稀之年的音乐家 Bruce Laland Faulconer 以《龙珠 Z》系列的作曲而闻名，最早参与的作品可至 20 多年前，直至 2018 年依然有作品产出。音乐生涯[著作等身](https://www.imdb.com/name/nm0269023/)、载誉无数的他在上周 Wikipedia 页面突然消失了。

移除的理由是在牛津大学出版社出版的《格罗夫音乐与音乐家辞典》（[Grove Dictionary of Music](https://www.oxfordmusiconline.com/grovemusic/)）上没有 Faulconer 的条目。

- Grove 在新媒体（比如日本动画）和独立媒体（alternative media）领域的音乐人收录上并不权威，更多的是收录与音乐历史与文化相关的条目；
- 一些作曲家在 Grove 上没有词条，但同样有 Wikipedia 条目；

结论大概率是某个编辑的一己私见，因为在 2018 年同样发生过类似事件。当年的诺贝尔物理学奖得主 Donna Strickland 在获奖前因为「名气不够」而无法拥有自己的 wiki 条目。回到 2012 年，知名作家 Philip Roth 在对自己的小说条目 《The Human Stain》提出异议时，被维基编辑告知他的反馈不是「可信来源」不予更改，后来 Roth 直接在纽约客上写了一封[公开信](https://www.newyorker.com/books/page-turner/an-open-letter-to-wikipedia)，详细地解释了该书和条目中冲突的地方。

到最后，Wikipedia 依然没有群组之外的公开且透明的运营反馈渠道。

→ 感受 Ted Gioia 的怒气

[How a Prominent Composer Lost His Wikipedia Page—and Got Entangled in Kafkaesque Nightmare Trying to Get it Back](https://tedgioia.substack.com/p/how-a-prominent-composer-lost-his)

附：写下本文时，Faulconer 的 wiki 条目已经复原。

---

2、第二条 Wikipedia 依然是主角。Rachel Gordon 这篇文章记录了 Wikipedia 是如何影响司法行为的。麻省理工学院计算机科学与人工智能实验室 (CSAIL) 和爱尔兰国立梅努斯大学的研究人员在爱尔兰的法律舞台开展了一项友好的压力测试：

- 让法律系学生撰写 150 多篇爱尔兰最高法院判决的百科条目，一半随机条目上传供法官、书记和律师等法职人员参考使用，作为实验组；
- 另一半条目置于离线状态，充当缺乏案例状态的条目，作为对照组；

实验想衡量两个标准：

- 这些案件是否会被之后的司法裁决文书引用？
- 法庭判决论点是否与新维基条目内容文风相似？

实验结果令人惊奇，Wikipedia 条目引用增加了 20%，具有相当的统计显著性。而且不出研究人员意料，下级法院（/ 地区法院）引用最多，高级法院（/ 巡回法院）其次，最高法院和上诉法院引用并没有增多（爱尔兰法律结构中，上级法院对下级法院有约束力）。维基百科的便利性还是很有吸引力的。

团队也使用 NLP（自然语言处理）分析裁判文书，发现了与百科条目相似的语义指纹。这意味着法官的判决意见有依赖于搜索相近案例结果导向，结案后的该文书又会被当做之后的相近案例参考。当源头（wiki）一旦出现信息操纵行为，那裂缝最终会越来越大。

→ 原文更详细说明

[How Wikipedia influences judicial behavior | MIT CSAIL](https://www.csail.mit.edu/news/how-wikipedia-influences-judicial-behavior)

---

3、披萨数学：一块 9 寸披萨，相当于多少块 5 寸披萨？当某个粗心的服务生回答 2 块的时候，就可以跟他科普 πr² 了。Flowing Data 做了一个可视化数据，来查看各尺寸披萨交换比例。比如 9 寸的披萨可以交换两个 7 寸的，也可以换两个 8 寸的。

![1670062343463.png](Scenes%20Weekly%20%2363.assets/1670062343463.png)

{上图：一块 9 寸可以换两个 8 寸披萨的话，挺赚}

→ 原文

[Pizza Exchange Rate](https://flowingdata.com/2022/07/26/pizza-exchange-rate/)

---

4、This Image Does Not Exist 与以往 This X Does Not Exist 网站不同，这是一个测验网站。判断 30 张图片是真人还是 AI 绘制 / 拍摄的。

→ 网站

[This Image Does Not Exist](https://thisimagedoesnotexist.com/)

---

5、Emoji Kitchen 是之前 Emojimix 的集合版，相当于点击一个 emoji 后把所有合成可能都展示出来，依旧很有意思。不过这个网站交互逻辑有点奇怪。

![1670062344709.png](Scenes%20Weekly%20%2363.assets/1670062344709.png)

{上图：选择幽灵后出现的一些改编 emoji}

→ 网站

[Emoji Kitchen Browser](https://emoji.supply/kitchen/)

---

6、One More Try 是一个实验性质的滑板记录短片，表现了完成一个成功的滑板动作背后所需要的艰辛。具体哪里「实验性质」可以直接查看原视频或者下面的预览 gif。

![1670062345966.gif](Scenes%20Weekly%20%2363.assets/1670062345966.gif)

{上图：一位粉色上衣白色下身的滑板选手在完成跳台阶动作}

→ 视频

[One More Try – an experimental skate video](https://vimeo.com/717945664)

---

> 我在维护一个自己订阅的 newsletters 列表，本通讯的内容也来源于此列表和其他信息聚合平台。这周新增了 4 个订阅，主要是因为开始整理邮箱。

→ [详见](https://fenx.work/design/newsletter) ([notion.com](http://notion.com))

→ [封面存档](https://figma.fun/f9e6Lk) ([figma.com](http://figma.com))

---

# 劳逸

![1670062348085.png](Scenes%20Weekly%20%2363.assets/1670062348085.png)

{上图：ULTRAKILL 横幅}

不同于以往 Doom-like 游戏，ULTRAKILL 扩展了「爽」的定义。在保留大 FOV + 高机动性的同时，增加了类似鬼泣的动作组合配置和风格评分。每把枪的技能和不同拳头（近战）的组合让游戏玩法非常灵活。

举个例子，游戏里有一把左轮手枪，技能是抛出硬币🪙，只要子弹或拳头击中在空中的硬币，硬币就会自动攻击敌人的弱点。抛出一堆硬币时，击中一枚会自动弹到其他硬币协同攻击敌人。瞄准手法有点像守望先锋里的艾什，但是更酷。

最重要的是游戏中还有弹反和近战回血的机制，大大降低了爽玩门槛，又不失操作上限，难得佳作。

→ [游戏获取](https://store.steampowered.com/app/1229490/ULTRAKILL/)

---

# 映像

现实拟像放映——

![1670062350231.jpeg](Scenes%20Weekly%20%2363.assets/1670062350231.jpeg)

{上图：不锈钢和胶合板组成的模块化厨房家具}

NPK01 Kitchen

© Chmara.Rosinke Studio

---

# 温故

→ Scenes Weekly #14

[Scenes Weekly | No. 14](https://mp.weixin.qq.com/s?__biz=Mzg3NzYwNDEzOQ%3D%3D&mid=2247484069&idx=1&sn=e3a33cd7a891a8777a2e8bac56063fd7&chksm=cf213ee1f856b7f76278fa95f5a8d8f0b2d1bbf42b43862ae6e196ce4d5b056175ab4912f200&token=923440544&lang=zh_CN#rd)

- Lyft 团队统一 segmented control 控件
- Clover app 公测
- 电商网站主页的八个容易被忽略的地方
- 多邻国游戏化（gamification）体验分享
- 产品定价策略
- Twitter 移除 Fleets
- Microsoft 新 emoji 图标

---

喜欢本文的话，欢迎分享、订阅。

第 62 期请[在此查看](./Scenes Weekly #62.md)。

本次封面使用了 Cotta 字体，灵感来源于夜市淘到的钩针编织小花。