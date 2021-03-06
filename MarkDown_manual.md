# **MarkDown语法**

## 标题

标题采用`#`符号定义，格式为`#+空格+标题名`（为了保持兼容性，中间加一个空格），其中标题级别采用`#`符号的数量进行区分，例如：

MarkDown语法格式如下：

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
```

展示格式如下：

# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题




### 标题另外一种用法

在标题名称后面加任意数量的`==`符号表示一级标题，标题名称后面加任意数量的`--`符号表示二级标题。例如：

一级标题======

二级标题-----------

**注意：** *此语法取决于你所使用的MarkDown解释器工具是否支持此语法，Typora不支持此语法，本文档采用Typora编辑的。*

## 段落

采用独立的空行进行上下两个段落的分割。例如：

MarkDown语法格式如下：

```
MarkDown功能很强大。
**** 空行 ****
我喜欢使用MarkDown。
```

展示格式如下：

***MarkDown功能很强大。***

***我喜欢使用MarkDown。***

**注意：**目前一些MarkDown编辑器如typora在非源代码模式编辑时直接回车就会自动加一行空行，源代码模式不会自动加空行。我们在用文本编辑器如vim、sublime或者Windows记事本等工具时需要自己添加一个空行，否则两个段落实际为一个段落。另外，段落不要用空格或者Tab缩进，除非在列表中。

## 换行符

换行符是在行的结尾加两个及以上的空格符。也有些采用`\`符号作为换行符，但不是所有的MarkDown解释器能识别这个用法。最优用法还是采用空格符。例如：

MarkDown语法格式如下：

```
第一行数据。    //此处有空格
另一行数据。
```

展示格式如下：

第一行数据。    
另一行数据。

换行符与段落的功能是区别的，段落之间行距较大，换行符在行结尾会有一个向下的箭头。

## 文本强调样式

###   ·文本加粗

文本加粗语法是在文本的前后各加两个星号（`*`）或者下划线（`_`）。例如：

MarkDown语法格式如下：

```
**星号加粗**
__下划线加粗__
```

展示格式如下：

**星号加粗**
__下划线加粗__

**注意：**为了保持各个MarkDown编辑器的兼容性，建议用星号符进行文本的加粗。

###   ·文本倾斜

文本倾斜是在文本的前后各加一个星号（`*`）或者下划线（`_`）。例如：

MarkDown语法格式如下：

```
*星号倾斜*
_下划线倾斜_ 
```

展示格式如下：

*星号倾斜*
_下划线倾斜_ 

**注意：**为了保持各个MarkDown编辑器的兼容性，建议用星号符将文本格式设置为斜体。

###   ·文本加粗并倾斜

文本加粗并倾斜是上述二者的叠加，即在文本的前后各加三个星号（`*`）或者下划线（`_`）。例如：

MarkDown语法格式如下：

```
***星号加粗并倾斜***
___下划线加粗并倾斜___ 
```

展示格式如下：

***星号加粗并倾斜***
___下划线加粗并倾斜___ 

**注意：**为了保持各个MarkDown编辑器的兼容性，仍然建议用星号符改变文本样式。

###  ·文本删除显示

文本删除显示即在一行文字中间有一横线（删除线），用法是文字前后各有2个`~`符号。例如：

MarkDown语法格式如下：

```
~~文字删除显示~~
```

展示格式如下：

~~文字删除显示~~

## 引用

引用的方式是在段落的前面加`>`符号，不需要加空格。例如：

MarkDown语法格式如下：

```
>此处为引用的内容。
```
展示格式如下：
> 此处为引用的文字内容。

###     ·多段引用

多段引用的方式是在两个段落中间的空行最前面加`>`符号。例如：

MarkDown语法格式如下：

```
>此处为引用段落1。
>
>此处为引用段落2。
```

展示格式如下：
>此处为引用段落1。
>
>此处为引用段落2。

###   ·嵌套引用

引用可以嵌套，嵌套的方式是在嵌套引用内容的最前面加`>>`符号。例如：

MarkDown语法格式如下：

```
>此处为主引用段落。
>
>>此处为嵌套引用段落。
```

展示格式如下：

>此处为主引用段落。
>
>>此处为嵌套引用段落。

###   ·引用与其他标记方法搭配使用

引用可以与MarkDown的其他格式标记方法搭配使用。例如：

MarkDown语法格式如下：

```
>#### 四级标题在引用中使用。
>**引用中字体加粗**
>>*嵌套引用字体倾斜*。
```

展示格式如下：

>#### 四级标题在引用中使用。
>**引用中字体加粗**
>
>>*嵌套引用字体倾斜*。

## 列表

可以将多个条目组成有序列表或者无序列表。

###   ·有序列表

有序列表的语法格式是`数字`+`.`+`空格`+`条目内容`。空格不可少。数字不一定是对应序列号，但列表的第一个条目一定得是1 ，展示出来的序列号是递增正确位置的序列号。如下面第二组例子中的数字`5`位于序列2的条目中，展示时会自动打印出`2`。例如：

MarkDown语法格式如下：

```
1. First item
2. Second item
3. Third item
4. Fourth item
```

展示格式如下：

1. First item
2. Second item
3. Third item
4. Fourth item

还可以：

```
1. First item
	1. Indent item
	2. Indent item
	3. Indent item
5. Second item
3. Third item
2. Fourth item
```

展示格式如下：
1. First item
	1. Indent item
	2. Indent item
	3. Indent item
5. Second item
3. Third item
2. Fourth item

**注意：**有序序列也可以采用`）`符号，不过有些MarkDown编辑器无法识别该符号，因此为了兼容性，建议还是使用`数字`+`.`+`空格`+`条目内容`的格式。（Typora就不支持该格式的用法）

###   ·无序列表

无序列表的语法格式是`-、+或者*符号中任一个`+`空格`+`条目内容`。利用空格或者Tab缩进可以嵌套列表。例如：

MarkDown语法格式如下：

```
- First item
- Second item
    - Indent item
    - Indent item 
    	- Indent item again
    	- Indent item again
- Third item
- Fourth item
```

展示格式如下：

- First item
- Second item
    - Indent item
    - Indent item 
    	- Indent item again
    	- Indent item again
- Third item
- Fourth item

**注意：**由于部分MarkDown解释器可能不支持多种标识符的混用，即一个无序列表中即有`-`符号，又有`+`或者`*`符号。为了保持兼容性，在一个无序列表中要统一使用同一个标识符。例如以下用法尽量不要使用：

```
- First item
+ Second item
* Third item
```

###   ·在列表中加入其它特性

可以再列表中加入其它特性，比如段落、引用等，语法格式是在其它特性文本前缩进4个空格或一个Tab。

####     ·列表中加入段落内容

MarkDown语法格式如下：

```
- 第一个列表条目内容
- 第二个列表条目内容

	这里需要在第二个列表中增加一个段落内容（根据段落语法格式要求，上一行和下一行都有空行）

- 第三个列表条目内容
```

展示格式如下：

- 第一个列表条目内容
- 第二个列表条目内容

	这里需要在第二个列表中增加一个段落内容（根据段落语法格式要求，上一行和下一行都有空行）

- 第三个列表条目内容

####     ·列表中加入引用特性

MarkDown语法格式如下：

```
- 第一个列表条目内容
- 第二个列表条目内容

	>这里需要在第二个列表中增加一个引用内容

- 第三个列表条目内容
```

展示格式如下：

- 第一个列表条目内容
- 第二个列表条目内容

	>这里需要在第二个列表中增加一个引用内容

- 第三个列表条目内容

####     ·列表中加入代码块

MarkDown语法格式如下：

```
1. 打开代码源文件
2. 查找代码中第10行的语法错误

		<html>
          <head>
            <title>Test</title>
          </head>

3. 更改代码中错误内容
```

展示格式如下：

1. 打开代码源文件
2. 查找代码中第10行的语法错误

		<html>
          <head>
            <title>Test</title>
          </head>

3. 更改代码中错误内容

####     ·列表中加入图片

语法格式同样是缩进4个空格或者1个Tab。例如：

MarkDown语法格式如下：

```
1. 打开图片存放位置

2. 选择要插入的图片

	![Images, test images](C:\Users\liu_y\Desktop\MarkDown_test.jpg)

3. 右键单击查看图片链接，并将链接放入指定位置
```

展示格式如下：

1. 打开图片存放位置

2. 选择要插入的图片

	![Images, test images](C:\Users\liu_y\Desktop\MarkDown_test.jpg)

3. 右键单击查看图片链接，并将链接放入指定位置

####     ·列表中加入列表

在有序列表中可以嵌套无序列表，反之亦然。例如：

MarkDown语法格式如下：

```
1. First item
2. Second item
3. Third item
	- Indent item
	- Indent item
4. Fourth item
```

显示格式如下：

1. First item
2. Second item
3. Third item
	- Indent item
	- Indent item
4. Fourth item

## 代码

让一个单词或者句子变成代码样式的方式就是前后使用``反引号（`）``。例如，Linux系统中打开目录的命令是`cd /home`。

###   ·反引号的转义

如果一段代码中含有反引号，我们就需要对它进行转义操作。用法是在代码前后采用两个反引号。例如：

MarkDown语法格式如下：

```
``我们的代码中已经含有单反引号了，`code`上下文。``
```

展示格式如下：

``我们的代码中已经含有单反引号了，`code`上下文。``

###   ·代码块

代码块的每行缩进至少4个空格或1个Tab即可。例如：

MarkDown语法格式如下：

```
    if(a<b)
        res = a;
```

展示格式如下：

    if(a<b)
        res = a;

如果上述每行缩进的方式太麻烦，还可以采用整段代码标注的方式，代码段前一行和后一行各用三个连续的反引号``（```）``或者三个连续的`~`符号（`~~~`）。例如：

MarkDown语法格式如下：

```

​```
if(a<b)
    res = a;
​```
```

展示格式如下：

```
if(a<b)
    res = a;
```

## 分割线

分割线的用户是采用3个或者3个以上的`*`符号、`-`符号或者下划线符`_`，使用时注意`---`所在行的前一行和后一行各一个空行。例如：

MarkDown语法格式如下：

```

---

```

展示格式如下：


---

## 链接

给文字插入超链接的语法是用方括号`[]`括住文字部分，后面紧跟着用圆括号`()`围起来的URL网址。例如：

MarkDown语法格式如下：

```
我常用的搜索引擎是：[bing搜索](https://cn.bing.com/)
```

展示格式如下：

我常用的搜索引擎是：[bing搜索](https://cn.bing.com/)

###   ·含标题的链接

可以给上述的链接增加一个标题，当用户将鼠标放在链接上时会出现一个标题提示，插入标题的语法是在上述URL后面增加一个双引号括起来的标题，双引号跟URL之间不要忘记空格。例如：

MarkDown语法格式如下：

```
我常用的搜索引擎是：[bing搜索](https://cn.bing.com/ "搜索效率高")
```

显示格式如下：

我常用的搜索引擎是：[bing搜索](https://cn.bing.com/ "搜索效率高")

###   ·URL网址或者邮件地址链接

如果不是为了给一段文字超链接，只是放一个可跳转的URL或者邮件地址的话，采用尖括号`<>`括起来即可。例如：

MarkDown语法格式如下：

```
<https://cn.bing.com/>

<liu_ya_nan@live.com>
```

展示格式如下：

<https://cn.bing.com/>

<liu_ya_nan@live.com>

###   ·文章内部标题的超链接

该功能的使用场景是将一个超链接指向本文章的某个地方，比如跳转到某个章节内容。语法规则是方括号`[]`中的内容采用反引号括住，后面括号中的内容为该章节的名称。例如：

MarkDown的语法格式如下：

```
Markdown语法中有序列表的使用方法[`点这里`](##·有序列表)。
```

展示格式如下：

Markdown语法中有序列表的使用方法[`点这里`](##·有序列表)。

**注意：**圆括号中的章节名称应该与原章节名称完全一样，比如上面标题中的`·`符号不能漏掉。另外标题级别标识符`##`后不再跟空格。


###   ·链接文本格式

链接文本格式跟[`文本强调样式`](##文本强调样式)中的用法一样，有加粗、斜体等样式。例如：

MarkDown语法格式如下：

```
我常用的搜索引擎是：[bing搜索](https://cn.bing.com/)

我常用的搜索引擎是：**[bing搜索](https://cn.bing.com/)**
```

展示格式如下：

我常用的搜索引擎是：[bing搜索](https://cn.bing.com/)

我常用的搜索引擎是：**[bing搜索](https://cn.bing.com/)**

## 图片

插入图片的语法规则是：感叹号`!`后紧跟一个方括号`[]`，方括号中可以是对图片的描述等，后面紧跟一对圆括号`()`，圆括号中存放图片的路径或者网络地址URL，还可以跟图片的标题等（放双引号中，鼠标放在图片上会显示），用法类似[`链接中标题用法`](##链接)。例如：

MarkDown语法格式如下：

```
![图片样例测试](C:\Users\liu_y\Desktop\MarkDown_test.jpg "MarkDown用法图片样例")
```

展示格式如下：

![图片样例测试](C:\Users\liu_y\Desktop\MarkDown_test.jpg "MarkDown用法图片样例")



###   ·图片超链接

图片具有超链接，点击图片可以跳转到指定网页。语法规则类似[`链接用法`](##链接)，只是中括号中的文字被图片的语法内容替换。例如：

MarkDown语法格式如下：

```
[![图片超链接](C:\Users\liu_y\Desktop\MarkDown_test.jpg "点击会跳转到bing首页")](https://cn.bing.com/)
```

展示格式如下：

[![图片超链接](C:\Users\liu_y\Desktop\MarkDown_test.jpg "点击会跳转到bing首页")](https://cn.bing.com/)



## 表格

建立表格的用法是采用3个或者3个以上的减号`-`符号创建每列的标题（首行），用管道符`|`分割各个列。例如：

MarkDown语法格式如下：

```
|姓名|年龄|性别|
|---|---|---|
|张三|20|男|
|李四|30|男|
```

展示格式如下：

|姓名|年龄|性别|
|---|---|---|
|张三|20|男|
|李四|30|男|

###   ·表格中文本对齐格式

表格中的文本可以指定对齐格式，左对齐、右对齐和中间对齐。语法规则是搭配冒号`:`符号的使用，左对齐时冒号在`---`符号的左侧，右对齐时冒号在`---`符号的右侧，中间对齐时冒号在`---`符号的两侧。例如：

MarkDown语法格式如下：

```
|姓名|年龄|性别|
|:---|:---:|---:|
|张三|20|男|
|李四|30|男|
```

展示格式如下：

|姓名|年龄|性别|
|:---|:---:|---:|
|张三|20|男|
|李四|30|男|

###   ·表格中文本样式

表格中的文本可以为其指定格式，比如文本加粗、倾斜、删除，链接、代码格式（只能使用单反引号格式的，不支持代码块的三个反引号的用法），不能将标题、引用、列表、分割线、图片或者HTML标签放在表格中。例如：

MarkDown语法格式如下：

```
|姓名|年龄|性别|
|:---|:---:|---:|
|**张三**|*20*|~~男~~|
|***李四***|***30***|~~男~~|
```

展示格式如下：

|姓名|年龄|性别|
|:---|:---:|---:|
|**张三**|*20*|~~男~~|
|***李四***|***30***|~~男~~|

###   ·表格中管道符`|`的反义

在表格中的文本中需要显示管道符`|`时，有两个方法：一是采用反斜杠进行反义，另外一个是直接用管道符的HTML字符代码（`&#124;`）管道符的ASCII码值是124 。以下是两种方法的例子：

MarkDown语法格式如下：

```
|字符|名称|使用场景|
|---|---|---|
|\||管道|新建表格|
|&#124;|管道|新建表格|
```

展示格式如下：

|字符|名称|使用场景|
|---|---|---|
|\||管道|新建表格|
|&#124;|管道|新建表格|

## 语法高亮

MarkDown支持代码块中的语法高亮，语法规则是在代码块前一行的三个反引号后紧跟代码语言名称。例如：

MarkDown语法格式如下：

```
​```c
if(a<b)
    res = a;
​```
```

展示格式如下：

```c
int a,b,res;
if(a<b)
    res = a;
```

## 脚注

添加脚注的语法规则是在中括号中采用插入符号（也叫脱字符）`^`和标识字段（数字或者文本都可以，但不能包含空格或者Tab），如：`[^1]`或者`[^note]`，标识字段要与脚注中解释内容的标识字段一一对应，且标识字段要唯一。脚注解释内容不一定要放在正文下方，可以放在文档的任何地方，但不能放在列表、表格和引用中。实际场景用法如下：

MarkDown语法格式如下：

```
1493年，哥伦布[^1]从美洲第一次返航，凯旋的队伍在塞维利亚[^塞维利亚]和巴塞罗那[^巴塞罗那]拥挤的街道间穿行，他向西班牙民众展示了无数的奇珍异宝——迄今为止的红色人种[^红色人种]。

[^1]: 意大利航海家，后受西班牙国王的委托企图寻找通往印度的新航线，1492年10月12日，人类的又一个星光闪耀时刻，他的船队发现一座被当地人称作“Guanahani”的小岛，因此哥伦布成为新大陆的发现者。

[^塞维利亚]: 西班牙西南部的内河港口及第四大城市，濒临大西洋。

[^巴塞罗那]: 西班牙东北部的港口城市，毗邻地中海。

[^红色人种]: 人种分类学上曾经长期存在的一个误解，即美洲印第安人从肤色上看是红色人种，后来发现其实是他们喜欢皮肤上涂红色颜料被误认为是红色皮肤。
```

展示格式如下：

1493年，哥伦布[^1]从美洲第一次返航，凯旋的队伍在塞维利亚[^塞维利亚]和巴塞罗那[^巴塞罗那]拥挤的街道间穿行，他向西班牙民众展示了无数的奇珍异宝——迄今为止的红色人种[^红色人种]。

[^1]: 意大利航海家，后受西班牙国王的委托企图寻找通往印度的新航线，1492年10月12日，人类的又一个星光闪耀时刻，他的船队发现一座被当地人称作“Guanahani”的小岛，因此哥伦布成为新大陆的发现者。

[^塞维利亚]: 西班牙西南部的内河港口及第四大城市，濒临大西洋。

[^巴塞罗那]: 西班牙东北部的港口城市，毗邻地中海。

[^红色人种]: 人种分类学上曾经长期存在的一个误解，即美洲印第安人从肤色上看是红色人种，后来发现其实是他们喜欢皮肤上涂红色颜料被误认为是红色皮肤。



###   ·脚注在HTML或者PDF文档中的展示样式

标识字段在HTML或者PDF文档中的展示格式是数字递增格式的，并非标识字段中的文字内容，Typora编辑器里展示的是标识字段的文本内容。另外脚注解释内容在HTML或者PDF文档中展示的地方在文档的结尾，Typora编辑器展示的地方是你编辑时存放的地方。例如：

**Typora脚注展示格式：**

![Typora脚注展示格式](C:\Users\liu_y\Desktop\Typora脚注展示格式.jpg "Typora脚注展示格式图例")

**HTML或PDF文档脚注展示格式：**

![HTML或PDF脚注展示格式](C:\Users\liu_y\Desktop\HTML或PDF脚注展示格式.jpg "HTML或PDF脚注展示格式图例")

![HTML或PDF脚注解释内容展示格式](C:\Users\liu_y\Desktop\HTML或PDF脚注展示格式2.jpg "HTML或PDF脚注解释内容在文档结尾展示")

## 任务列表

MarkDown支持用复选框表示任务列表，语法规则是每行文本前加`- [ ] `（未选中）或者`- [x] `（已选中），中括号前后均有空格，如果是未选中中括号中为空格，否则是`x`字母。例如：

MarkDown语法格式如下：



展示格式如下：

计算机经典书籍待读：

- [x] Unix环境高级编程

- [ ] Unix网络编程

- [ ] TCP/IP详解

- [ ] 高性能MySQL


## 转义字符

若文档中需要显示以上各个语法中用到的字符，比如星号`*`、`+`、`-`等，需要进行转义才可以。转义方法同其他计算机语言，采用反斜杠`\`符号实现。例如：

MarkDown语法格式如下：

```
\* 如果没有反斜杠进行转义这行文本会变成一个列表
```

展示格式如下：

\* 如果没有反斜杠进行转义这行文本会变成一个列表

需要进行转义的字符清单如下：

|字符|名称|使用场景|
|:---|:---|:----|
|\\|反斜杠|转义其他字符|
|\`|反引号|插入代码|
|\*|星号|文字加粗或者倾斜，无序列表功能，分割线|
|\_|下划线|文字加粗或者倾斜，无序列表功能，分割线|
|\{\}|大括号||
|\[\]|中括号|插入图片|
|\<\>|尖括号|URL或者邮件地址链接|
|\(\)|圆括号|链接、插入图片|
|\#|井号|标题级别|
|\+|加号|无序列表|
|\-|减号|无序列表、分割线|
|\.|点号|有序列表|
|\!|感叹号|插入图片|
|&#124;|管道|新建表格|





