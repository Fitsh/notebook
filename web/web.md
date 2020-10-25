## html

<p>标签用于在HTML文档里定义一个段落。

浏览器在显示<p>段落时，将在其前后分别插入一个空白行。这些空白是由浏览器在呈现网页时自动加入的，你也可以用样式表来指定显示多少空白。


标签描述<i>定义斜体文本<b>定义粗体文本<big>定义大字体文本<small>定义小字体文本



<br>标签用于插入一个换行符。

<br>是一个空元素（empty element），也就是说，它不需要结束标签。

<br>标签不支持任何事件属性。

<dl>标签用于创建一个定义列表（definition list）。

<dl>标签是与<dt>和<dd>联合使用的。<dt>用于创建定义列表中的一项（术语），<dd>用于为定义列表中的项创建描述。

<li>标签用于定义列表项。

有序列表（<ol>）和无序列表（<ul>）均用<li>标签来定义列表项。

<s>和<strike>标签用于定义已被删除的文本。

<span>标签本身并不产生任何视觉效果。

它只是提供一种途径，令你可以对文档中的一部分进行引用。

这样，你便可以引用部分文本，并对它们设置样式，或用JavaScript对它们进行处理

<u>标签用于定义带下划线的文本。

### 瞄点定位

通过创建瞄点链接，用户可以快速定位到目标内容。

瞄点定位分为两步：

```markdown
1. 使用"<a href="#id名">链接文本 </a>
2. 使用相应的id名标注跳转目标的位置
```

### base标签

base标签可以设置整体链接的打开状态

单标签，位于head,设置所有链接的打开方式，target=_blank|_self

### 特殊字符

| HTML 原代码 | 显示结果 | 描述                   |
| ----------- | -------- | ---------------------- |
| \&lt;       | <        | 小于号或显示标记       |
| \&gt;       | >        | 大于号或显示标记       |
| \&amp;      | &        | 可用于显示其它特殊字符 |
| \&quot;     | "        | 引号                   |
| \&reg;      | ®        | 已注册                 |
| \&copy;     | ©        | 版权                   |
| \&trade;    | ™        | 商标                   |
| \&ensp;     |          | 半个空白位             |
| \&emsp;     |          | 一个空白位             |
| \&nbsp;     |          | 不断行的空白           |

有序列表

ol li

无序列表

ul li

自定义列表

dl dt dd

```html
<dl>
    <dt>北京</dt>
    <dd>aaa</dd>
    <dd>adad</dd>
    <dd>aaa</dd>
</dl>
效果：
北京
	aaa
	adad
	aaa
```

表格：

"<table>
<tr>
    <th>ada</th>
    <th>adaa</th>

</tr>

<tr>

<td></td>

</tr>

</table>"

td只是一个可以容器，里面可以放任何元素

使用表格进行布局时，可以将表格分为头部、主体和页脚，具体如下所示：

<thead></thead>:用于定制表格的头部，必须包含于<table></table> 标签中，一般包含网页的logo和导航等头部信息。

<tbody></tbody>:用于定义表格的主体。位于<table></table>标签中，一般包含网页中除头部和底部以外的其它信息。

"<table>

<thead>

<tr>
    <th>ada</th>
    <th>adaa</th>

</tr>

</thead>

<tbody>

<tr>

<td></td>

</tr>

</tbody>

</table>"

表格标题：

caption

"<table><caption>标题</caption></table>"

合并单元格

跨行合并：rowspan, 跨列合并：colspan

从上到下，从左到右

```html
<table>
    <tbody>
    <tr>
    	<td>A</td>
        <td>B</td>
        <td rawspan="2" >C</td>
    </tr>
     <tr>
    	<td>D</td>
        <td>E</td>
    </tr>
    </tbody>
</table>
```

input:

type:test、password、radio、checkbox、button、submit、reset、image、file 

name、value、checked src size， maxlength

可以通过相同name来设置一组radio。

<input type="radio" name="sex"/>男 <input type=radio" name="sex"/>女

type="image" src为图片位置，此为图片按钮

label标签：

绑定一个表单元素，当点击label标签时，被绑定的表单元素可以获取输入焦点

for属性规定与哪个表单元素绑定

```html
<label for="male">Male</label>
<input type="radio" name="sex" id="male" value="male" />
```

也可以不用for属性，直接label包含input元素即可 

textarea控件(文本域)

如果需要输入大量的信息，就需要用到<textarea></textarea>

可以创建多行文本输入

cols\rows属性控制列和行

下拉菜单：

 ```html
<select>
    <option selected="selected">点击选择</option>
    <option>选项1</option>
    <option>选项2</option>
</select>
 ```

表单域：<form></form>

属性：action  method name

## html5

- header 定义文档的页眉头部

- nav 定义导航链接的部分

- footer：定义文档或节的页脚底部

- article：定义文章

- section:定义文档中的节(section,区段 )

- aside 定义其所处内容之外的内容 侧边

- datalist 标签定义选项元素，与input元素配合使用，来定义 input 可能的值，datalist 及其选项不会被显示出来，它仅仅是合法的输入值列表

- fieldset 可将表单内的相关元素分组，打包，与legend搭配使用

  fieldset 元素可将表单内的相关元素分组。

  <fieldset> 标签将表单内容的一部分打包，生成一组相关表单的字段。

  当一组表单元素放到 <fieldset> 标签内时，浏览器会以特殊方式来显示它们，它们可能有特殊的边界、3D 效果，或者甚至可创建一个子表单来处理这些元素。

  <fieldset> 标签没有必需的或唯一的属性。

  <legend> 标签为 fieldset 元素定义标题。

```html
<input id="myCar" list="cars" /> input里用list
<datalist id="cars"> datalist用id来实现和input链接，输入内容显示相应的提示
  <option value="BMW">
  <option value="Ford">
  <option value="Volvo">
</datalist>

```

```html
 <fieldset>
    <legend>健康信息</legend>
    身高：<input type="text" />
    体重：<input type="text" />
  </fieldset>
```

input 新增类型

```html
<form action="">
        邮箱<input type="email" name="" id=""> <input type="submit" value="提交"><br /><br />
        手机号码<input type="tel" name="" id=""> <input type="submit" value="提交"><br /><br />
        网址<input type="url" name="" id=""> <input type="submit" value="提交"><br /><br />
        数字<input type="number" name="" id=""> <input type="submit" value="提交"><br /><br />
        搜索框<input type="search" name="" id=""> <input type="submit" value="提交"><br /><br />
        拖动滑块<input type="range" name="" id=""> <input type="submit" value="提交"><br /><br />
        时间<input type="time" name="" id=""> <input type="submit" value="提交"><br /><br />
        日期<input type="date" name="" id=""> <input type="submit" value="提交"><br /><br />
        日期时间<input type="datetime" name="" id=""> <input type="submit" value="提交"><br /><br />
        几年几月<input type="month" name="" id=""> <input type="submit" value="提交"><br /><br />
        几年几周<input type="week" name="" id=""> <input type="submit" value="提交"><br /><br />
   		颜色<input type="color" name="" id=""> <input type="submit" value="提交"><br /><br />
    </form>
```

[HTML5](http://www.100sucai.com/)的input标签新增了很多属性，
新增属性一：autoconmplete
autoconmplete可以赋值为 on 或者 off。当为 on的时候，浏览器能自动存储用户输入的内容。当用户返回到曾经填写过值的页面的时候，浏览器能把用户写过的值自动填写在相应的input框里。
现在很多网站都实现了这个功能，不过基本都是用php来实现的。用了这个属性，无疑可以减少很多前端和后台的交流量和工作量。该元素需要name属性，需要提交按钮
新增属性二：autofocus
autofocus 可以赋值为 autofocus，也就是在页面加载完成的时候自动聚焦到这个input标签，自然 type="hidden"的时候是不能用的。 这个也是一个比较常见的效果，至今为止的实现方法是用js。在页面加载完时执行聚焦操作，现在也被一个属性搞定了。
可以想象，一个页面至多只有一个input标签会设置 autofocus，否则必然不会达到预期效果。因为不可能同事聚焦在两个input上。
新增属性三：required
input的有一个强力新增属性，免去验证的麻烦。可以赋值为 required。
比如用户注册页面的用户名和密码都是必填的，只要设置一个required就可以了。而在以前是需要js来验证或者后台验证的。
注意：这里required属性是需要用户来填写的，所以TYPE是button、submit、reset、image等等不需要用户填写选择的类型是不可以使用这个属性的。
新增属性四：placeholder
这个新增属性也是非常使用，用在type= text email等等类型的时候，提示用户输入信息的格式或者内容等等。这个效果在之前也是需要js来实现的。是一种比较常见的效果：

新增属性五：multiple 多选，多文件上传

新增属性六：accesskey 规定激活（使元素获取焦点）元素的快捷键，采用alt+字母的形式

 HTML5 INPUT新增属性
新增属性五：新增list属性---联想框效果
这个属性显示类似于百度[搜索框](http://www.100sucai.com/web/jquerytexiao/zaixiankefu)那种联想框效果，也是非常实用的一个属性。
注意从这个属性使用的特点：需要有对应的datalist标签；datalist子标签option支持 value和lable两个属性；list的属性值要和datalist的id一致。

多媒体标签：

- embed 标签定义嵌入的内容
- audio 播放音频
- video 播放视频

audio

| 属性                                                         | 值       | 描述                                                         |
| :----------------------------------------------------------- | :------- | :----------------------------------------------------------- |
| [autoplay](https://www.w3school.com.cn/tags/att_audio_autoplay.asp) | autoplay | 如果出现该属性，则音频在就绪后马上播放。                     |
| [controls](https://www.w3school.com.cn/tags/att_audio_controls.asp) | controls | 如果出现该属性，则向用户显示控件，比如播放按钮。             |
| [loop](https://www.w3school.com.cn/tags/att_audio_loop.asp)  | loop     | 如果出现该属性，则每当音频结束时重新开始播放。               |
| [muted](https://www.w3school.com.cn/tags/att_audio_muted.asp) | muted    | 规定视频输出应该被静音。                                     |
| [preload](https://www.w3school.com.cn/tags/att_audio_preload.asp) | preload  | 如果出现该属性，则音频在页面加载时进行加载，并预备播放。如果使用 "autoplay"，则忽略该属性。 |
| [src](https://www.w3school.com.cn/tags/att_audio_src.asp)    | *url*    | 要播放的音频的 URL。                                         |

control 属性供添加播放、暂停和音量控件。

在<audio> 与 </audio> 之间你需要插入浏览器不支持的<audio>元素的提示文本 。

”<audio> 元素允许使用多个 <source> 元素. <source> 元素可以链接不同的音频文件，浏览器将使用第一个支持的音频文件“

```html
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
您的浏览器不支持 audio 元素。
</audio>
```

video

"<video> 元素提供了 播放、暂停和音量控件来控制视频。"


同时 <video> 元素也提供了 width 和 height 属性控制视频的尺寸.如果设置的高度和宽度，所需的视频空间会在页面加载时保留。如果没有设置这些属性，浏览器不知道大小的视频，浏览器就不能再加载时保留特定的空间，页面就会根据原始视频的大小而改变。

"<video> 与</video> 标签之间插入的内容是提供给不支持 video 元素的浏览器显示的。"

"<video> 元素支持多个 <source> 元素. <source> 元素可以链接不同的视频文件。浏览器将使用第一个可识别的格式："

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
您的浏览器不支持Video标签。
</video>
```

## css

#### css 字体样式

font-size: 字体大小

font-family: 字体

css unicode 字体

- 在css中设置字体名称时，写中文是可以的，但在文件编码（g2312、utf-8）不匹配时会产生乱码
- 方案:
  - 使用英文代替
  - 在css中unicode编码来写字体名避免错误

font-weight 字体粗细

font-style字体风格

font 综合设置字体，简写属性在一个声明中设置所有字体属性，可以按顺序设置如下属性：

- font-style

- font-variant

- font-weight

- font-size/line-height

- font-family

  可以不设置其中的某个值，比如 font:100% verdana; 也是允许的。未设置的属性会使用其默认值

:thumbsup:常用技巧：

- 网页中字体普遍：14px+
- 尽量使用偶数数字字号，老式浏览器用奇数有bug
- 各种字体之间必须使用英文状态下的逗号隔开
- 中文字体名需要加英文状态下的引号，英文字体名不需要引号，当需要设置英文字体时，英文字体名必须在中文字体名前面
- 如果字体名中包含空格，#， $等符号，该字体必须加英文状态下的单或双引号，如"Times New Roman"
- 尽量使用系统默认字体，保证任何用户的浏览器能正确显示

#### 注释

/* 注释*/

#### 选择器

##### 标签选择器（标签即元素）

##### 类选择器：使用"."(英文点号)进行标识，后紧跟类型

:thumbsup:小技巧:

- 长名称或词组可以使用中横线来为选择器命名
- 不建议使用"_"下划线来命名css选择器
  - 浏览器兼容问题（比如使用_tips的选择器命名，在IE6是无效的
  - 能良好的区分js变量命名，（js变量命名使用"_")
- 不要纯数字、中文等命名，尽量用英文字母来表示

##### 多类名选择器

给标签指定多个类名，达到更多的选择目的

- 样式效果和类名先后顺序无关，受css样式书写的上下顺序有关

- 各个类名之间用空格隔开

##### id选择器

使用"#"进行标识，后面紧跟id，id是唯一的，只对应某个具体元素

##### 通配符选择器

用"*"号表示，能匹配页面中的所有元素

##### 伪类选择器

向某些选择器添加特殊效果，比如给链接添加特殊效果比如选择第n个元素

使用":"冒号

下面的E可为标签，.类名，#id等

链接伪类选择器：

- E:link 未访问的链接

- E:visited 已访问的链接

- E:hover 鼠标移动到链接上

- E:active 选定的链接

  写的时候，顺序尽量不要颠倒

结构（位置）伪类选择器(CSS3)

- E:first-child 匹配父元素的第一个子元素E
- E:last-child 匹配父元素的最后一个子元素E
- E:nth-child(n): 匹配父元素的第n个子元素E, n: odd even n（所有） 2n(所有偶数) 3n(3，6，9)...,  8指定第8个
- E:nth-last-child(n):匹配父元素的倒数第n个子元素E。不论元素类型，从最后一个计数，n可以是数字、关键字、或公式

目标伪类选择器：

E:target 匹配相关URL指向的E元素。

与瞄点定位结合使用

#### css外观属性

color 属性规定文本的颜色，支持预定义的颜色值、十六进制、RGB代码

line-height 属性设置行间的距离（行高）。不允许使用负值。该属性会影响行框的布局。在应用到一个块级元素时，它定义了该元素中基线之间的最小距离而不是最大距离。

line-height 与 font-size 的计算值之差（在 CSS 中成为“行间距”）分为两半，分别加到一个文本行内容的顶部和底部。可以包含这些内容的最小框就是行框。

原始数字值指定了一个缩放因子，后代元素会继承这个缩放因子而不是计算值，属性值单位有三种，像素、相对值em或百分比%.

一般行距比字体大7.8像素就可以了

text-align 属性规定元素中的文本的水平对齐方式。该属性通过指定行框与哪个点对齐，从而设置块级元素内文本的水平对齐方式。通过允许用户代理调整行内容中字母和字之间的间隔，可以支持值 justify；不同用户代理可能会得到不同的结果。可能的值：left、right、center、justify、inherit

text-indent 属性规定文本块中首行文本的缩进。

**注释：**允许使用负值。如果使用负值，那么首行会被缩进到左边

可能的值

| 值       | 描述                                      |
| :------- | :---------------------------------------- |
| *length* | 定义固定的缩进。默认值：0。               |
| *%*      | 定义基于父元素宽度的百分比的缩进。        |
| inherit  | 规定应该从父元素继承 text-indent 属性的值 |

1em就是一个汉字的宽度

letter-spacing 属性增加或减少字符间的空白（字符间距）。

该属性定义了在文本字符框之间插入多少空间。由于字符字形通常比其字符框要窄，指定长度值时，会调整字母之间通常的间隔。因此，normal 就相当于值为 0。

**注释：**允许使用负值，这会让字母之间挤得更紧。

word-spacing 属性增加或减少单词间的空白（即字间隔）。针对英文，对于中文来说无效

该属性定义元素中字之间插入多少空白符。针对这个属性，“字” 定义为由空白符包围的一个字符串。如果指定为长度值，会调整字之间的通常间隔；所以，normal 就等同于设置为 0。允许指定负长度值，这会让字之间挤得更紧。

**注释：**允许使用负值。

颜色半透明(css3)

```css
color: rgba(r, g, b, a)  a是alpha的意思  a 位于0~1
```

文字阴影(css3)

text-shadow 设置文本阴影

```css
text-shadow:水平位置 垂直位置 模糊距离 阴影颜色
```

| 值       | 描述           |
| -------- | -------------- |
| h-shadow | 必须，允许负值 |
| v-shadow | 必须，允许负值 |
| blur     | 可选           |
| color    | 可选           |

一般网页不用纯黑，用淡黑色字，3c3c3c