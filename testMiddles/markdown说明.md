### 概述、宗旨
---

Markdown 的目标是实现「易读易写」。

可读性，无论如何，都是最重要的。一份使用 Markdown 格式撰写的文件应该可以直接以纯文本发布，并且看起来不会像是由许多标签或是格式指令所构成。总之， Markdown 的语法全由一些符号所组成，这些符号经过精挑细选，其作用一目了然。Markdown 的列表看起来，嗯，就是列表。Markdown 的区块引用看起来就真的像是引用一段文字，就像你曾在电子邮件中见过的那样。

### 段落、标题、区块代码
---

一个`段落`是由一个以上的连接的行句组成，而一个以上的空行则会划分出不同的段落（空行的定义是显示上看起来像是空行，就被视为空行，例如有一行只有空白和 tab，那该行也会被视为空行），一般的段落不需要用空白或换行缩进。

在行首插入 1 到 6 个 # ，对应到`标题 1 到 6 阶`。区块引用则使用`> 角括号`。

**markdown语法:**
```
这行开头什么都没有，就是一个段落。

> 这就是一个区块，有一个空行是为了分行。
>
> 否则的话，
> 就会连起来。
>
> ## 区块内同样可以使用标题
>
> > 同样也可以使用别的markdown语法。
```

**效果为：**

这行开头什么都没有，就是一个段落。

> 这就是一个区块，有一个空行是为了分行。
>
> 否则的话，
> 就会连起来。
>
> ## 区块内同样可以使用标题
>
> > 同样也可以使用别的markdown语法。

### 修辞和强调
---
Markdown 使用星号和底线来标记需要强调的区段。

**Markdown 语法:**

    这是 *强调*。
    这也是 _强调_。
    这是**斜体**。
    这也是__斜体__。

**效果为：**

这是 *强调*。
这也是 _强调_。
这是**斜体**。
这也是__斜体__。

### 列表
---
无序列表使用星号、加号和减号来做为列表的项目标记，这些符号是都可以使用的，使用加号：

    + Candy.
    + Gum.
    + Booze.

**效果为：**

+ Candy.
+ Gum.
+ Booze.

有序的列表则是使用一般的数字接着一个英文句点作为项目标记：

    1. Red
    2. Green
    3. Blue

**效果为：**
1. Red
2. Green
3. Blue

### 链接
---
Markdown 支援两种形式的链接语法： 行内 和 参考 两种形式，两种都是使用角括号来把文字转成连结。

行内形式是直接在后面用括号直接接上链接：

    这是一个 [链接](http://lanthree.com/).

**效果为：**

这是一个 [链接](http://lanthree.com/).

参考形式的链接让你可以为链接定一个名称，之后你可以在文件的其他地方定义该链接的内容：

我喜欢的网站有很多，例如 [伯乐在线][1]、
[花瓣][2]、[在线作图][3]等等。

[1]: http://blog.jobbole.com/
[2]: http://huaban.com/
[3]: https://www.processon.com/

### 图片
---

图片的语法和链接很像。

行内形式（title 是选择性的）：

```
![alt text](/dist/img/photo1.png "title")
```

**效果为：**

![alt text](/dist/img/photo1.png "title")

同样，链接也可以有`title`，图片也有参考形式。

### 代码
---
代码分为行内形式和区块形式两种，行内形式只需要用\`包括起来：

    `markdown`很方便。

效果为：

`markdown`很方便。

如果要建立一个已经格式化好的代码区块，只要每行都缩进 4 个空格或是一个 tab 就可以了，或者上下添加三个紧挨着的\`符号：

```
GET /font-awesome/css/font-awesome.css 304 3.320 ms - -
GET /mypublic/stylesheets/SourceSansPro.css 304 3.772 ms - -
GET /ionicons/css/ionicons.min.css 304 3.658 ms - -
GET /dist/css/AdminLTE.min.css 304 3.476 ms - -
GET /dist/css/skins/skin-blue.min.css 304 3.346 ms - -
```
如上就是效果了。

### 表格
---

表格的书写有多重方式，这里只说明最为简单的一种：

```
表头 1 | 表头 2
-------- | --------
单元格 1   | 单元格 2
单元格 3   | 单元格 4
```

**效果为：**

表头 1 | 表头 2
-------- | --------
单元格 1   | 单元格 2
单元格 3   | 单元格 4
