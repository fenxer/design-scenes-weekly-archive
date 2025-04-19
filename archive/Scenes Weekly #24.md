# Scenes Weekly #24

2021-09-26

本系列为微博 @Design_Scenes 的每周总结以及其他杂事。

本周出现：Figma、Noi Grotesk、Amplitude、Epicene、Innovation by Design、Play (App)、Podcast、Matrix、Nate Piekos、Rolling Stone、Photoshop Beta、Design in Nature、edo moji、Ben Sanders、Hoxton Campus

---

# **周三**

**Figma** 最近对复制粘贴这一基础功能进行了全方位的更新，更新的基本原则为尽量保持粘贴前元素的位置和粘贴后在当前焦点能看到目标。官方又为此又准备了一个 playground，有时间可自行体验 ↓

[Figma](https://www.figma.com/community/file/1019677205098431673/Copy-and-paste-playground)

没时间的话可以——

- 首先 Figma 增加了 Paste here 选项，没有快捷键，只能右键弹出。顾名思义在当前位置以元素的左上角为基准粘贴，无视相对位置。
- Paste 不会像普通复制粘贴一样，插入到 Auto Layout 里，而是独立的浮在上面。
- 现在选择 Frame 中某个元素，可以在多个 Frame 中批量粘贴，相当实用。
- Paste to replace 功能可以粘贴替代某些现有的元素位置，无视元素本身大小，保留 Constraints。同样支持批量复制和批量替换。
- 缩小视图后复制某个元素，再放大视图后于另一个地方粘贴元素，元素出现在当前视图的中央，不会再像之前样跑回原本的元素上方了。
- 复制 Frame 里的某个元素，移到没有该 Frame 的视图区域再粘贴时，同样元素出现在当前视图的中央。
- 复制 Frame 里的某个元素，移到露出一部分 Frame 的视图区域再粘贴时，会复制到 Frame 里。
- 复制一个视图里很大的元素，粘贴后会根据视图区域做出调整。
- 复制一个 Frame 中的 Group 的一个元素，粘贴外层 Frame 时，会保留元素在 Group 中的相对位置，也就是总会保持父层的相对位置。
- 复制一个 Frame 里的元素，粘贴到 Group 中，会保留元素在 Frame 中的相对位置。
- 对于勾选 Clip Content 的 Frame，复制 Frame 视觉外逻辑内的元素时，保持不变。
- 复制 Frame 逻辑上的元素时，粘贴到 Frame 里不再乱跑而是在原位置，这个也很实用。
- 一些其他复制粘贴相关的 tips。

![640 (3).jpeg](Scenes%20Weekly%20%2324.assets/640%20(3).jpeg)

---

Noi Grotesk 字体的丰富 Stylistic Set，轴变换时的细节修正都给人留下了深刻的印象。视频为 Studio Feixen 配备的可变字体微动效演示。

详见微博 ↓

[https://weibo.com/6728914621/KzlGeaDfJ](https://weibo.com/6728914621/KzlGeaDfJ)

现实情况是，可变字体在用户界面设计的实践中还没踏出一大步。

---

# **周五**

之前分享过 Amplitude 团队对于可易用性颜色系统的构建见解，为了解决人眼视觉上的亮度问题，他们采用了定比型颜色分级这一复杂算法 ↓

[https://weibo.com/6728914621/JFTCv94y1](https://weibo.com/6728914621/JFTCv94y1)

这个问题很多团队都遇到过，比如这次 Postmark 团队分享了 **Accessible Palette** 工具，来尝试更方便地这个问题。他提倡放弃使用 HSL / HSV 颜色模型来构建颜色系统，改用CIELAB / L*a*b* 模型。熟悉 Ps 的朋友应该能看出来 a* 是绿-红轴，b* 是蓝-黄轴，L是亮度，亮度越极端，人眼能区分的颜色越少，符合常识认知。即便是有限的 sRGB 色域也可以形象体现出来。

由此，Accessible Palette 这个基于 Chroma.js 的工具用处就体现出来了。

![640.jpeg](Scenes%20Weekly%20%2324.assets/640.jpeg)

原文（内含工具地址） ↓

[Accessible Palette: stop using HSL for color systems | Wildbit](https://wildbit.com/blog/2021/09/16/accessible-palette-stop-using-hsl-for-color-systems)

---

# **摘录**

这周看过的一些——

> One of the truly mind-flaying things about China is those occasional moments when you read a news story about the country and it cites a particular city that you have never heard of and you Google it and it’s literally bigger than London and it’s just AN Other ‘second tier’ city which is considered ‘largely unremarkable’.

—— Web Curios 17/09/21

---

# **杂事**

1、Klim Type Foundry 于本月21日发布了新的巴洛克风格字体 **Epicene**。

![640.png](Scenes%20Weekly%20%2324.assets/640.png)

Epicene 的灵感来自于18世纪的 J-F. Rosart 和 J.M. Fleischmann 两位排版大师的作品，大写的 A、W、E、T 充斥着古典衬线气息，小写的 a、p、g 又有新古典衬线的味道，刚柔并济。按照 Klim 的说法——

*Culturally, Epicene says one thing: typefaces have no gender.*

官网和样本查看 ↓

[Klim Type Foundry · Epicene Collection](https://klim.co.nz/collections/epicene/)

设计过程 ↓

[Klim Type Foundry · Epicene design information](https://klim.co.nz/blog/epicene-design-information/)

---

2、Fast Company 一年一度的 **Innovation by Design** 公布了获奖名单。

![640 (1).png](Scenes%20Weekly%20%2324.assets/640%20(1).png)

眼熟的 MTA、汉堡王品牌重塑等也在其中。

查看所有获奖者 ↓

[Fast Company's 2021 Innovation by Design Awards | Fast Company](https://www.fastcompany.com/innovation-by-design/2021)

---

3、以在手机上做交互为卖点的 native 应用 **Play**，之前上架了 App Store。但目前只能查看案例，想要创作自己的原型，依然需要邀请。

![640 (2).png](Scenes%20Weekly%20%2324.assets/640%20(2).png)

即便如此， Play 对复杂交互的处理依然值得考察学习一番。有时间的话应该会写写感受。

官网 ↓

[Home](https://www.createwithplay.com/)

---

4、HELEN LI 探讨了 Spotify 和 Apple 等西方播客提供商如何像国内播客学习，特别是面向创作者一方，包括如何如何改善主播与听众的生态以及最重要的盈利手段等。

不过我不听播客，所以也不多说了。详见 ↓

[What Spotify and Apple can learn from Chinese podcasting apps](https://restofworld.org/2021/what-spotify-and-apple-can-learn-from-chinese-podcasting-apps/)

---

5、@iquilezles 分享了黑客帝国的色调公式激起了大家的算法欲望：

![640 (3).png](Scenes%20Weekly%20%2324.assets/640%20(3).png)

对于像我一样不懂代码的人来说，可以用曲线去实现。下面拿 Ps 举例，载入图片后打开**曲线**，RGB 通道分别调整为：

```other
R = 255 * pow( (R/255), 3/2 )
G = 255 * pow( (G/255), 4/5 )
B = 255 * pow( (B/255), 3/2 )
```

我是以输入横坐标120为准算的，对应 RGB 输出纵坐标为82、139和82。

如下图曲线：

![640 (4).png](Scenes%20Weekly%20%2324.assets/640%20(4).png)

拿去和原推的图对比，应该没错了。最后点击齿轮图标存个预设，挺有意思的。

原推评论可以看到更多 ↓

[登录 Twitter，关注inigo quilez](https://twitter.com/iquilezles/status/1440847977560494084)

---

6、**Nate Piekos** 教你美漫对话气泡排版：

![640 (5).png](Scenes%20Weekly%20%2324.assets/640%20(5).png)

摘自他即将出版的 **Essential Guide to Comic Book Lettering**。

---

7、时隔17年滚石杂志更新了 **500 Greatest Songs of All Time ——**

![640 (6).png](Scenes%20Weekly%20%2324.assets/640%20(6).png)

榜单 ↓

[The 500 Greatest Songs of All Time](https://www.rollingstone.com/music/music-lists/best-songs-of-all-time-1224767/kanye-west-stronger-1224837/)

歌单（网易云）↓

[「2021版」滚石杂志:史上最伟大的500首歌曲](https://music.163.com/playlist?id=5286208836&userid=47339997)

---

8、Photoshop Beta 即将支持 **Unified Text Engine**，用于更好地支持中东、东亚地区语言支持。如图避头尾、标点溢出等高级排版功能，提高了 Ps 排版上限。

![640 (7).png](Scenes%20Weekly%20%2324.assets/640%20(7).png)

新闻源 ↓

[Announcing the availability of Unified Text Engine in Photoshop Beta](https://community.adobe.com/t5/photoshop-beta-discussions/announcing-the-availability-of-unified-text-engine-in-photoshop-beta/m-p/12381978)

---

9、《自然中的设计》第二卷中的 XCVIII 图版。

![640 (8).png](Scenes%20Weekly%20%2324.assets/640%20(8).png)

© [books.google.co.uk](http://books.google.co.uk)

---

10、A is for 博客的这篇文章介绍了各种江户文字（edo moji）——寄席文字、勘亭流、相扑文字、髭文字、笼文字、角字。其实还有提灯文字没有提及……

带有配图的原文 ↓

[A is for](https://aisforfonts.com/edomoji)

---

11、致力于图像脱离语境的 **Ben Sanders** 办过一个展览，在放大了现实里30倍的瓶盖上进行艺术创作。

![640 (9).png](Scenes%20Weekly%20%2324.assets/640%20(9).png)

©  Ben Sanders

看惯了日常不起眼的瓶盖，现在变成了艺术的主要载体，让人眼前一亮。

查看更多瓶盖图案 ↓

[Bottle Caps — Ben Sanders Studio](https://bensandersstudio.com/Bottle-Caps)

---

12、**Hoxton Campus** 是伦敦的四栋用于办公出租服务的建筑。

![640 (10).png](Scenes%20Weekly%20%2324.assets/640%20(10).png)

Anagram 在做品牌设计时，将这四栋楼的占地空间配上两个字母 O 拟人化，如下图。

![640 (11).png](Scenes%20Weekly%20%2324.assets/640%20(11).png)

并置于真实的场景中，光影和反射细节都很到位。

查看动起来的图形们 ↓

[Hoxton Campus – ANAGRAM](https://anagram.london/work/hoxton-campus/)

---

# **劳逸**

不会一直工作——

![640 (1).jpeg](Scenes%20Weekly%20%2324.assets/640%20(1).jpeg)

本周白金了破晓传说，推荐给所有喜欢 JRPG 的人。然后等待审判之逝的盘。

---

封面使用了 MetamorBit 字体。

