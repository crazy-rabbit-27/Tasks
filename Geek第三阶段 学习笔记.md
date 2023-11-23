# HTML学习笔记

- 常用标签

1.标题标签一共6个网页标签，<>中加h+n（表示1~6）,其中n代表以级标题，h是head的缩写，标题文字会<u>变粗</u>，<u>字号会变大</u>，标题独占一行。

2.段落标题html被分成很多部分，<p>是一个段落的标题，p表示paragaraph的缩写。文本会根据浏览器大小自动换行，而且段落间也有空隙。

3.换行标签，强制换行，<bt/>单标签，b表示break缩写，<bt/>单标签是另起一行，和段落应该不太一样。

4.<div>和<span>标签，这两个标签没有什么语义，差不多是用来放东西的。

前者用来布局，一行只能放一个,容量大；后者标签一行上可以放多个，容量小。

5.超链接标签，<a>即使一个页面跳转到另一个页面。<a htef = "跳转目标"；target = "目标窗口弹出方式"></a>

hetf:用于指定连接目标的地址（这是必要属性）

target：用于指定链接页面的打开方式，_self为默认，_blank为在新的窗口打开。

6.<button>按钮标签，用于创建一个可点击的按钮。

- 块级元素与内联元素

[块级元素和内联元素学习地](https://blog.csdn.net/lwf3115841/article/details/129052250?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522170057661016800186519955%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=170057661016800186519955&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-1-129052250-null-null.142^v96^pc_search_result_base7&utm_term=html%E5%9D%97%E7%BA%A7%E5%85%83%E7%B4%A0%E5%92%8C%E8%A1%8C%E5%86%85%E5%85%83%E7%B4%A0&spm=1018.2226.3001.4187)

- 标签样式

[HTML标签样式](https://blog.csdn.net/Bianca427/article/details/124980762?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522170057699416800186599710%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=170057699416800186599710&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-1-124980762-null-null.142^v96^pc_search_result_base7&utm_term=HTML%E6%A0%87%E7%AD%BE%E6%A0%B7%E5%BC%8F&spm=1018.2226.3001.4187)

# CSS学习笔记

- 作用

  [css了解视频](https://www.bilibili.com/video/BV1bW411R7hg/?spm_id_from=333.337.search-card.all.click)

  CSS样式决定了网页的外观

  CSS可以设置页面上某些元素的外观：字的颜色，字的大小，字的对齐方式，背景颜色或者背景图像等

  通过上述了解，我认为css就像是一个设计师，让整个页面有个性化。

- 选择器

1. 通用选择器：可以同时选中页面中所有的元素。语法 *{}

2. 元素选择器：可以根据标签的名字来从页面中选取指定的元素。语法 标签名{}     

   e.g.比如p则会选中页面中的所有p标签，h1会选中页面中的所有h1标签.

   3.类选择器：可以根据元素的class属性值选择元素。语法 className{}

​       比如 .hello会选中页面所有class属性为hello的元素。

​    4.ID选择器：ID选择器，可以根据元素的id属性值选取元素。语法：#id{}

- 盒子模型

   1.内容区域的宽、高：数字+px

   2.边框：单个取值连写，取值之间用空格隔开（快捷键bd+tab、solid实线、dashed虚线、dotted点线）

   3.边框单方向设置：border-方位词 

e.g.border-bottom 盒子大小=width/height +边框线+内边距， 多值写法，永远都是从上开始顺时针转一圈，如果值不够多，看对面取值；padding最多取4个值，取两个值上下一样，左右一样。

​      4.定位:

静态定位:设置灵位方试:属性值static；设置偏移值:属性名水平方同left/right； 属性值:数字+px;；垂直方向top/bottom

相对定位（相对自已原位置移动）：代码:position:relative; 占有原来的位置；仍然具有原标签显示模式持点；改交位置参照园召原来位置

绝对定位:position: absolute; 先找到已定位的父级，如果有就以这个父级为参照物进行定位；有父级，但父级没有定位，则以浏览器窗口为参照进行定位。

（特点：脱标，不占位；改变标签的显示模式特点，具体行内块特点，一行共存，宽高生效，父级相对定位，子级绝对定位。）

固固员位:固灵到浏览器某位置position:fixed; 脱标，不占位；改位置参考浏览器窗口；具备行内块特点，要设置宽高！！

​       5.常用的布局方式

普通布局：每一个网页元素都有一个display属性，用于确定该元素的类型，每一个元素都有默认的display属性值。比如div元素，它的默认display属性值为"block",成为“块级”元素(block-level);而span元素的默认 display属性值为'inline",称为“行内”元素。

学习来源：[来源地](https://zhuanlan.zhihu.com/p/65353887)

浮动布局：指定一个元素应沿其容器的左侧或右侧放置，允许文本和内联元素环绕它。float属性用于定位和格式化内容，例如让图像向左浮动到容器中的文本。float的值有: · left-元素浮动到其容器的左侧 right-元素浮动到其容器的右侧·none-元素不浮动(将仅显示在文本中出现的位置)。这是默认的inherit-元素继承其父元素的浮点值。

学习来源：[来源地](https://segmentfault.com/a/1190000014554601)

弹性布局：Flexible Box模型，通常被称为flexbox，是一种一维的布局模型。它给flexbox的子元素之间提供了强大的空间分布和对齐能力。容器默认存在两根轴:水平的主轴(main axis)和垂直的交叉轴(cross axis)。
容器有以下属性: 
 flex-direction-属性决定主轴的方向(即项目的列方向) flex-wrap-定义设置换行模式flex-flow-定义了项目在主轴上的对齐方式justify-content-定义项目在交叉轴上如何对齐align-items-定义项目在交叉轴上如何对齐·align-content-定义了多根轴线的对齐方式。

学习来源：[来源地](https://juejin.cn/post/6844904116141948936)

定位布局：给元素设置postion属性后，就可以定义该元素的top,bottom, left,right四个属性。当然postion的值不同，对应的top，bottom, left, right这四个属性的值代表的含义也不相同position属性用来指定一个元素在网页上的位置，一共有5种定位方式: · static-静态relative-相对定位fixed-固定定位absolute-绝对定位sticky-粘性定位

学习来源：[来源地](:https://developer.mozilla.org/zh-CN/docs/Web/CSS/position)

表格布局：display:table/table-row/table-cell... 有两种方式使用表格布局-HTML Table(stable>标签)和CSS Table(display:table等相关属性)。HTML Table是指使用原生的<table>标签，而CSS Table是指用CSS属性模仿HTML表格的模型。

学习来源：[display:table的几个用法:](https://blog.51cto.com/u_4048786/3205160)

​                  [CSStable布局大法](https://segmentfault.com/a/1190000007007885)

栅格布局：格布局将网页划分成一个个网格，可以任意组合不同的网格，做出各种各样的布局。

学习来源：[Gird布局](https://juejin.cn/post/6854573220306255880)

多列布局：多列布局声明提供了一种多列组织内容的方式，正如你在一些报纸中看到的那样。这篇文章介绍怎么使用这一特性。

学习来源：[来源地](ttps://www.zhangxinxu.com/wordpress/2019/01/css-Css3- columns-layout/)

- 伪类

anchor伪类
在支持CsS的浏览器中，链接的不同状态都可以以不同的方式显示

a:link{color:#FFO000:3/*未访问的链接*

a:visited {color:#00FFO03/*已访问的链接*

 a:hover fcolor:#FFO0FF/*鼠标划过链接*

 a.active{color:#0000FF/*已选中的链接*

易错：

1.在CSS定义中，a:hover必须被置于a:link和a: visited之后，才是有效的。

2.在CsS定义中，a:active必须被置于a:hover之后，才是有效的。

3.伪类的名称不区分大小写。

CSS :first-child伪类
您可以使用:first-child伪类来选择父元素的第一个子元素。

易错：在E8的之前版本必须声明<！DOCTYPE>, 这样:first-child才能生效。

# JavaScript学习笔记

[JS详细学习地](https://zh.javascript.info/)

- 数据类型

字符串：string字待串类型:通过引1号"包裹的数据都叫字符串(推荐用单引号)。在JS中加了引号就是字符串类型输出引号内内密，因此量不能加引号！引号成对使用，单引|号/双引号可以互相嵌套，(内双外单，外双内单)；必要时转义符可以直接让其输出引号+加号可以拼接字待串。

document.write(我今年+age+岁了)输出age赋值数据我今年n岁了

数字：Number类型用来表示整数和浮点数，最常用的功能就是用来表示10进制的整数和浮点数。

Number表示的数字大小是有限的，范围是: -±1.7976931348623157e+308。 如果超过了这个范围，则会返回±Infinity。
·NaN,即非数值(Not a Number)是一个特殊的数值，JS中当对数值进行计算时没有结果返回，则返回NaN。
数值的转换。
·有三个函数以把非数值转换为数值:Number()、parselnt() 和parseFloat()。
· Number()可以用来转换任意类型的数据，而后两者只能用于转换字符串。
parselnt()只会将字符串转换为整数，而parseFloat()可以转换为浮点数。

布尔：·也被称为逻辑值类型或者真假值类型。布尔型只能够取真(true)和假(false)两种数值。除此以外，其他的值都不被支持。其他的数据类型也可以通过Boolean(函数转换为布尔类型。

Null：Null类型是第二个只有一个值的数据类型，这个特殊的值是null。从语义上看nul表示的是一个空的对象。所以使用typeof检查null会返回一个object。undefined值实际上是由nul值衍生出来的，所以如果比较undefined和null是否相等，会返回true；

Undefined：Undefined类型只有一个值，即特殊的undefined。在使用var声明变量但未对其加以初始化时，这个变量的值就是undefined。例如: 
var message; 
message的值就是undefined。
需要注意的是typeof对没有初始化和没有声明的变量都会返回undefined.

数组：数组基本使用:能够声明数组月能够获取里面的数据(一组数据)；let数组名=[数据1，数据2，.., 
数据n一1] （下标从0开始排）

1. 数组是按顺序保存，所以每个数组都有自己的编号

2. 数组中数据编号也叫索引或下标

3. 数组可以存储任意类型的数据

   

# 了解HTML/CSS/JavaScript三者之间的关系

HTML：是用于创建网页结构的标记语言。它提供了一系列的标签和元素，用于定义网页的结构、内容和布局。

CSS：是一种样式表语言，用于描述网页的外观和样式。通过CSS，可以对HTML元素进行样式化，包括字体、颜色、布局等。

JavaScript：是一种用于给网页添加交互功能的脚本语言。它可以操作HTML元素、处理用户输入、与服务器进行交互等。JavaScript可以在网页加载完毕后修改和操作HTML和CSS，从而实现动态网页效果和用户交互。

简单说，HTML用于创建网页的结构，CSS用于提供网页的样式，而JavaScript用于为网页添加动态效果和交互功能。

[学习地1](https://www.bilibili.com/video/BV1MX4y1a77m/?spm_id_from=333.337.search-card.all.click)

[学习地2](https://www.bilibili.com/video/BV1HZ4y1V7wm/?spm_id_from=333.337.search-card.all.click)