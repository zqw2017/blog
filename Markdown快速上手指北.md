# Markdown快速入门指北（win）  

![](https://res.cloudinary.com/darryl/image/upload/v1484757640/jsej3zvqvivt3cq3wcat.jpg)

>We believe that writing is about content, about what you want to say – not about fancy formatting.
>
>我们坚信写作写的是内容，所思所想，而不是花样格式。
>— *Ulysses for Mac*  

## Hello,MarkDown  

Markdown应该是这两年写作编辑里的一股新秀了，从程序员到网站小编等群体的日常办公中都能看到markdown的身影，与word这类富文本编辑器不同，Markdown 是一种用来写作的轻量级「标记语言」，它用简洁的语法代替排版，往往排版在键盘输入文字的时候就一起完成了，这使得人们可以专注于内容和文字本身，这也是markdown的核心思想所在：简洁、高效、易读易写。

 ## 说得好，那我该用什么软件呢



我用的是win平台下的[typora](https://typora.io/)，有时也会用github出的[atom](https://atom.io/),前者用于文字编辑，后者用来版本控制和push到github

###  我的系统不是win...

那我很难给出具体的建议，不过听说MacOS对markdown的支持是更好的，可以自行去网上搜索相关的软件

### 我想用手机/ipad码字...

安卓系统上听说纯纯写作还可以  
ios的话，熊掌记，Ulysses，支持markdown的app很多  
有电脑的话不建议在移动端码字。   

##  markdown怎么用啊  

在开始介绍语法前先要解释的是，不像word这类所见即所得的文字编辑工具，markdown对于文字的处理分为渲染前和渲染后，类似于网页浏览器的工作方式，将html代码进行解析和渲染，最终得到我们所看到的网页，所以不要问为什么我写的markdown没有呈现想要的效果，我用的typora是实时预览的，但很多软件是需要手动打开预览窗口（渲染出的效果预览），建议同时打开编辑窗口和预览窗口，可以实时检查排版。  

### 标题  

使用 **#** +空格可表示 1-6 级标题， 

![](https://zakery.oss-us-west-1.aliyuncs.com/usr/article/markdown/pc8Vg9eG96.png)  

### 段落  

markdown里的换行是两个以上的空格+回车或者空一行来实现的，Typora 在空格与换行部分主要是使用 [CommonMark](http://www.commonmark.cn/w/) 作为标注规范。与前文提到的 GFM 一样，CommonMark 也是比较流行的 Markdown 语言规范（解析器）之一。

![](https://cdn.sspai.com/2019/05/24/5c2fbaa53b27666a7fd0b07ac3e100bf.png?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1)

### 列表

#### 有序列表  

有序列表使用数字并加上 **.** 号来表示

 ![](https://zakery.oss-us-west-1.aliyuncs.com/usr/article/markdown/BxCdDFYXIi.png)

#### 无序列表  

无序列表使用星号(*****)、加号(**+**)或是减号(**-**)作为列表标记

![](https://zakery.oss-us-west-1.aliyuncs.com/usr/article/markdown/KaTg3FlKZj.png)

#### 列表嵌套

列表嵌套只需在子列表中的选项添加四个空格即可  
![](https://zakery.oss-us-west-1.aliyuncs.com/usr/article/markdown/m5ZastuMnX.png)

### 引用  

有时需要引用别人文章的一段话，可以在段落开头使用 **>** 符号 ，然后后面紧跟一个**空格**

![引用](http://ww3.sinaimg.cn/large/6aee7dbbgw1effezhonxlj20e009c3yu.jpg)

### 代码  

如果是段落上的一个函数或片段的代码可以用反引号把它包起来（**`**）  

1. 行内代码:用 **`** 或 **``** 括起代码,不会实现代码高亮。如：   

```
  `printf()` 函数
```

 		效果：  
		`printf()`

2. 代码块：输入 **```** 后并输入语言名，换行，开始写代码，Typora 就会自动帮你实现代码高亮。如：  

   ```
   ​``` #include<stdio.h>
   	printf("hello,world");```
   ```

   ``` c
   	#include<stdio.h>
   	printf("hello,world");
   ```

### 链接

链接使用方法如下：

```
[链接名称](链接地址)
或者
<链接地址>
```

如：

```
这是一个链接 [baidu](https://www.baidu.com)
```

效果：

这是一个链接 [baidu](https://www.baidu.com)  

### 图片

markdown里图片插入和word有点不一样，需要提供图片的链接或者是本地路径，如果文章写来是为了留在电脑上自己看的话用本地路径即可，如果是发布到网上的，必须先上传到图床然后获取对应的图片链接，否则图片会失效  Markdown 图片语法格式如下：

```
![文本](图片地址)

![文本](图片地址 "可选标题")
```

- 开头一个感叹号 !

- 接着一个方括号，里面放上图片的替代文字

- 接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。

  使用实例：

  ```
  ![哔哩哔哩图标](https://i0.hdslb.com/bfs/archive/1be2fd76cc98cdc6a595c05c3134fbf937a1c126.png)
  ```

![哔哩哔哩图标](https://i0.hdslb.com/bfs/archive/1be2fd76cc98cdc6a595c05c3134fbf937a1c126.png)

### 表格

Markdown 制作表格使用 **|** 来分隔不同的单元格，使用 **-** 来分隔表头和其他行。

语法格式如下：

```
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |
```

| 表头   | 表头   |
| ------ | ------ |
| 单元格 | 单元格 |
| 单元格 | 单元格 |

**我们可以设置表格的对齐方式：**

- **-:** 设置内容和标题栏居右对齐。
- **:-** 设置内容和标题栏居左对齐。
- **:-:** 设置内容和标题栏居中对齐。

实例如下：

```
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |
```

| 左对齐 | 右对齐 | 居中对齐 |
| :----- | -----: | :------: |
| 单元格 | 单元格 |  单元格  |
| 单元格 | 单元格 |  单元格  |

### 脚注

某段话结尾右上角标有数字标记，页面底部进行注释的写法。你可以在需要插入脚注标号的位置写 `[^ number ]` ，再在下方通过 `[^ number ]:` 在文档中插入脚注。注意不要遗漏了脚注编号 `number` 前后的空格。

[^ 1]:www.baidu.com

baidu[^ 1]

### 字体和分割线

Markdown 的粗体和斜体非常简单，用两个 `*` 包含一段文本就是粗体的语法，用一个 `*` 包含一段文本就是斜体的语法。分割线的语法只需要三个 `*` 号

**这里是粗体** *这里是斜体*  

***

## 结语

学到这儿markdown的日常使用已经没有问题，如果以前用word的话刚转来markdown会有些不适应，适应几天就好，还是那句话，不要为了工具而使用工具，使用什么样的工具取决于你自己的需求，不要盲目跟风，也不要无脑吹，认清工具的本质灵活运用。之后有空的话会更一篇高级使用的方法，内容包括但不限于markdown里流程图的绘制，数学公式的输入，html标签的使用，祝各位都能在写作中有所收获。