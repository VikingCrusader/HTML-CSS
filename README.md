# HTML-Learning
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
