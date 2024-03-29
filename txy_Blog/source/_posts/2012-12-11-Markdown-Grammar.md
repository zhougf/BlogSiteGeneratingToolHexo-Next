---
layout: post #布局
title: Markdown语法 #标题
date: 2012-12-11 14:15:00 +0800 #建立日期
updated: 2012-12-11 14:15:00 +0800 #更新日期
comments: true #开启文章的评论功能
tags: [个人博客, 使用说明, 工具, markdown, 平板文件, 教程] #标签（不适用于分页）
categories: instructions #分类（不适用于分页）
permalink: #覆盖文章网址
---

[下载思维导图文件](https://docs.google.com/file/d/0B7UFT4BR96esZTBxR3dOV3JnbHc/edit?usp=sharing)

# 致谢

- 站在这位 *[巨人](http://markdown.tw/)* 的肩膀上 
- 作者[samrain](http://samrain.github.com/)

# 直接使用HTML

- 一般来说直接使用

- 特殊：块标签必须在前后加上空白，例如：`div`,`table`,`pre`,`p`

- 注意：块标签中的MD语法无效，而段标签中有效，例如：`span`,`cite`,`del`

# 特殊字符处理(`<`和`&`)

- 可以直接使用

- 在code范围内转换为`&lt;`和`&amp;`

# 段落

- 一个以上相连接的句子组成

# 换行

- 一个以上的空行会转化为`p`

- 如果想要`br`换行，必须在行尾加上2个以上空白再回车

# 标题

- 底线形式(Setext)

        在标题文字后另起一行，写上特殊符号

        一阶标题用`=`，二阶标题用`-`

        符号数量随便

- Atx形式

        在标题文字行首加入1到6个`#`，代表1到6阶

        注意：`#`后必须加一个空格

# 引用文字

- 在段落的第一行或者每行前面加上`>`

- 可以有层次，只要根据层数加上不同数量的`>`

- 可以使用其他md语法，比如标题、清单和程序区块等

# 清单

- 无序

        在行首添加*或+或-再加上空格

- 有序

        数字加英文句号加空格

        数字不影响顺序，最好从1开始(方便写作过程中调整语句顺序后忘记修改数字编号)

- 可以包含段落

        段落必须缩排4个空格/1个tab

- 可以包含引言

        引言的符号`>`必须缩排4个空格/1个tab

- 可以包含程序

        必须缩排8个空格/个tab

- 如果不想使用分块，但是又必须出现数字+句号，那么在句号前加反斜杠"\"

# 链接

- 行内

        直接把文字和URL写在一行中

        方括号把文字括起来，后面紧跟小括号把URL括起来

        例如：This is [an example](http://example.com/ "Title")

- 参考

        URL统一定义，文字后跟的是ID

        第一个方括号把文字括起来，后面紧跟第二个方括号把id括起来

        例如：This is [an example][id] reference-style link.

        id可以放在文章任意地方(建议放在末尾)，方括号把id括起来+冒号+空白+url+双引号/小括号括起来title内容。如果title太长，可以放到下一行。例如：[id]: http://example.com/ "Optional Title Here"

        省略用法:如果文字和id一样，那么在第二个括号中就不要写id了。留一个空括号。例如：[Google][]            [Google]: http://google.com/

# 图片

- 行内

        感叹号+方括号把图片替代文字括起来+小括号把URL括起来+空格+双引号括起来的title文字

        例如：![Alt text](/path/to/img.jpg "Optional title")

- 参考

        感叹号+第一个方括号把文字括起来+第二个方括号把id括起来

        例如：![Alt text][id]

        id可以放在文章任意地方(建议放在末尾)，方括号把id括起来+冒号+空白+url+双引号/小括号括起来title内容。如果title太长，可以放到下一行。例如：[id]: http://www.taosteel.com/static/images/logoTaosteel.gif "Optional title attribute"

# 分隔线

- 在一行中用三個或以上的星號、減號、底線來建立一個分隔線，行內不能有其他東西。你也可以在星號中間插入空白

# 程序代码

- 缩排4个空白/1个tab

- md语法不会被转换

- 如果标记一小段可以用反引号包起来，如果要显示反引号，那么在前后放入一个空格，然后用多个反引号包围

# 强调

- 用`*`或`_`包围的文字,符号必须成对出现

- 一对符号转译为`em`(斜体)，二对符号转译为`<strong>`

# 自动链接

- 网站链接/邮件地址，用尖括号括起来，例如：<https://drive.google.com> <samrainhan@gmail.com>

# 用反斜杠来插入特殊符号

<pre>
\   反斜線
`   反引號
*   星號
_   底線
{}  大括號
[]  方括號
()  括號
#   井字號
+   加號
-   減號
.   英文句點
!   驚嘆號
</pre>