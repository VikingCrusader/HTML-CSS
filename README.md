# HTML and CSS -Learning
My Daly Learning of HTML

Day 1 Marz 26 HTML B站网课P1-20
1.处理图像<img src="" title="" alt="" width="" height="" border=""/>
2.标题<h1></h1> to <h6></h6> 从大到小
3.段落<p></p>
4.强制换行<br />
5.文本编辑
  加粗 <strong></strong>
  倾斜 <em></em>
  
  删除线 <del></del>
  下划线 <ins></ins>
6.<div></div> <span></span>都是布局标签，前者就是独占一行，后者是集中到一行
一个案例 体育新闻 还有reddit复制的day1.html，当练习了。

Day2 Marz 27 HTML B站网课21-29
1.相对路径，linux讲过，上一级文件夹../ 下一级文件夹/
2.超链接标签<a href="" target=""></a> target默认_self，本页面，可以设置_blank，另弹出窗口
3.href外部链接必须以https开头，内部链接可以是xxxx.html
4.图片链接<a href="" target=""><img=src""></a>
5.下载链接<a href="xxx.zip"></a>
6.锚点链接<a href="#A"></a> <h1 id="A"></h1>
7.注释 <!--我是注释-->

Day3 Marz 28
完成了综合案例--圣诞树和圣诞老人
B站网课30--40
1.表格
<table align="center/left/right" border="1" cellpadding="20" cellspacing="0" width="1000"></table>
aligh对齐方式 border边界宽度 cellpadding字距离边框的距离 cellspacing单元格之间的距离 width表格宽度
<table></table>里面<thead></thead> <tbody></tbody>
行<tr></tr> 表头<th></th> 里面元素<td></td>
2.合并单元格
先找到要合并的单元格，目标单元格是最左边或最上边的单元格（rowspan跨行 最上边，colspan跨列 最左边）
然后呢在目标单元格的标签里写rowspan=""或colspan="" 例如<td rowapan="2"></td>
最后手动删除多余的格子
3.无序列表
<ul>
  <li></li>
  <li></li>
</ul>

Day4 Marz 29 b站网课 41--50
1.有序列表
<ol>
  <li></li>
  <li></li>
</ol>
2.自定义列表
<dl>
  <dt></dt>
  <dd></dd>
  <dd></dd>
</dl>
3.表单
<form></form>
4.input
<form>
  <input> input是个单标签，input必须包含在form里面
</form>
<input type="" name="" value="" checked="" maxlength="">
5.input的type属性
text 纯文本输入
password密码输入
radio单选 需要name
checkbox多选 需要name
6.name 区分，用于单选多选
7.value 默认值
8.check="checked"默认选上（用于单选多选）
9.maxlength="10"最大长度

Day5 Marz 30 b站网课 51--60
继续<input>的type
file 文件上传
submit 提交按钮
button 按钮 配合javscript启动脚本
reset重置
<label for=""><input id=""></label> for和id一样的前提下，可以点击图标或者文本就选中
<textarea>文本框
做了一个综合案例 表单+表格+列表
html完结 明天css

Day6 CSS第一天 b站网课 61--70
选择器
标签选择器
p {
  attributes
}
类选择器
一定不要忘记点"."
<style>
  .red{
    background-color: red;
  }
</style>
<body>
  <div class="red">jjj</div>
</body>
id选择器
<style>
  #red{
    background-color: red;
  }
</style>
<body>
  <div id="red">jjj</div>
</body>
实际开发中，设计样式用类多，id一般用于和js一起使用

Day7 April 1st
CSS b站网课 71-80， 310 remain
1.通配符选择器
*{
  Attributes
}
这个选择器能把所有的标签选中，包括html，body，div，p等
2.CSS字体属性
字体库 font-family 
字体大小 font-size 注意px
字体样式 font-style italic意大利斜体 normal正体
字体粗细 font-weight 没有单位
font连写：style weight size family 注意顺序，可以一行解决，不过初学者还是算了 慢慢来 欲速则不达
3.CSS文本装饰
color：预设置颜色 十六进制 rgb
十六进制-#001100 from PS
rgb 最方便
预设置也很简单
文本对齐：text-align：left/right/center
装饰文本: text-decoration: none/ underline/ overline/ linethrough
none可以删除下划线，主要用于链接
underline主要用于突出

Day 8 April 2 B网课 81--100 CSS
1.CSS文本缩进 text-indent:20px or 2em
2.行间距 ；line height：20px emmt简写lh20px
3.CSS引入方式 三种 在此不多赘述
值得一提的是 若把CSS分文件编写，<link rel="stylesheet" href="my.css">直接link+tab自动出来，不用记
4.Chrome调试工具 cmd+opt+J element 右上角
5.Emmet语法 多敲就会了
6.复合选择器
子元素选择器   ol li {} 选择所有li
亲儿子选择器，只选择亲的 .nav a{} 只选择.nav下一级的，孙子级别的不选

Day9 April 3 B网课 101--110 CSS
1.并集选择器
div,
p{
  样式语句
}
2.链接伪类选择器
a:link {} 选择所有未被访问的链接
a:visited {} 选择所有访问过的链接
a:hover {} 选择鼠标悬停的链接
a:active {} 选择鼠标按下但还未松开的链接
LVHA的顺序不能乱 最常用的就是给a设置一个样式，给hover设置一个样式
3.:focus伪类选择器
选择有光标的表单元素编辑
input:focus{
  background-color:pink
}
<input type='text'>
4.元素显示模式
块元素<div></div> <p></p> <h></h> <ol></ul>
自己独占一行，高度宽度内边距都可以控制，宽度默认是浏览器宽度100%，是一个盒子，里面可以放行内元素或者块元素
行内元素
<a><span>
一行可以放多个元素，高度宽度不能直接设置，默认宽度就是本身内容的宽度，只能容纳文本或者其他行内元素
行内块元素
<img /> <input /> <td />
一行可以放多个这种元素，可是大小可以控制

Day10 April4 B站网课 111--128 CSS
1.显示模式的转换 Display
行内转块：Display:block;
块转行内：Display:inline;
转化为二者特性兼具的模式：Display:inline-block;
2.单行文字垂直居中的技巧
设定line-height和height相同
3.CSS背景颜色
background-color
4.背景图片
background-image url()
5.背景大小
background-size xxpx xxpx
6.背景位置 
俩坐标 前面是x后面是y 可以用left right top bottom center这种也可以用px 分别指距离左边框和上边框的距离，可以混合
7.背景图片常用于小logo的放置，因为它比较方便控制位置
8.网页大背景直接写在body{}里面
9.背景固定 background-attachment:scroll or fixed 背景图片是否随文字滚动
10.背景色设置半透明：rgba（0，0，0，0.3）最后面的值是透明度，0是透明1是完全不透明，文字不受影响

Day11 April 5 B站网课 129--140 CSS
1.CSS的层叠性，相同选择器针对同一个元素 下面的比上面的优先级高
2.继承性 子标签继承父标签的特性 例如文本颜色 字号 行高等
3.优先级 同一个元素指定多个选择器时 选择器相同执行层叠性  选择器不同  执行优先级根据权重 !important>style行内修改>ID>class>标签>继承，其中继承的权重为0，权重可以叠加，记住那个表格
4.盒子模型-网页布局的核心就是用CSS摆盒子
5.border边框 border: 10px solid red 三个元素 顺序不重要 样式：solid dashed dotted比较常用
6.可以用border-left/right/top/bottom指定某个边的样式如果写在下面某个边的样式，则会覆盖，利用层叠性。

Day12 April 6 B站网课 141--150 CSS
1.border边框合并
border-collapase
2.padding复合写法: 顺序上左下右，只写一个：四周padding一样 写两个，第一个上下第二个左右
3.padding会撑大盒子，（提前声明盒子的宽高的前提下）如果需要测量盒子，宽高减去padding的长度
4.margin 外边距，以一个为基准写，连写顺序和padding一模一样

Day13 April 7 B站网课 151--160 CSS
1.块级盒子水平居中:margin:0 auto;
行内或者行内块：text-align:center;
2.避免外边距塌陷：用于大盒子套小盒子，如果修改小盒子的margin或者padding会影响大盒子，这样的话只能用overflow:hidden
3.消除内外边距，便于排版，建议每次排版前都这样做
*{
    padding:0;
    margin:0;
}
4.PS基本操作 多用就熟了 用于测量图片大小和提取颜色
5. width：100% height同理，用于调整内部盒子大小和外部盒子的某个边同样大

Day14 April 8 B站网课 161--170 CSS
1.listul去掉远点: list-style:none;
2.圆角边框 border-radius:10px; 其中后面是半径 可以用这个做圆形盒子
3.盒子阴影 box-shadow 10px 10px 10px 10px black;
4.文字阴影 text-shadow 同上

Day 15 April 9 B站网课 171--180 CSS
就学了float排版
注意点：
1.浮动元素脱离标准流
2.顶端对齐
3.浮动的元素具有行内块元素特性
做了三个练习

Day 16 April 10
练习了一个网页布局的案例
1.如果需要整个页面不填满，居中，可以在外面套一个大的container，然后设置container的样式令其居中，margin：0 auto
2.多重选择器，中间逗号隔开，不是空格
3.html和css同时保存，live server才会刷新
Day 17 April 11
清除浮动，目的是为了解决盒子不方便给高的情况，子盒子不会跑到父盒子的外边
1.额外标签法，不常用
在每个行结束时都添加一个块级元素例如<div class = "clear" ></div> style写 .clear{clear:both} 不常用 因为麻烦
2.给父元素添加 overflow:hidden简洁
3.clearfix，复制以下代码：
.clearfix:after {
    content: "";
    display: block;
    height: 0;
    clear: both;
    visibility: hidden;
}
给html文件的父盒子添加：
<div class="clearfix"></div>
就行了，这样万无一失
4.双伪元素，一个道理，记住clearfix就行了。

Day17 April 12
常见图片格式
jpg/jieg 产品类图片
gif 动图
png 保持透明背景
pds PS设计稿

Day18 April13
学成在线准备工作
明天准备素材 后天学PS
大后天开始制作网页

Day19 April 14 准备了素材
