#Markdown

段落之间空一行。同一段落不同行，在行结束时输入两个空格。

##标题

标题有6个等级，对应#,##,...###### ，一般使用前3级。

```
#这是第一级，文章的标题
##这是第二级，文章主要部分的大标题
###这是第三级，二级标题下面一级的小标题
####这是第四级，谨慎使用四级标题，尽量避免出现，保持层级的简单和防止出现过于复杂的章节。  
```

效果：

#这是第一级，文章的标题
##这是第二级，文章主要部分的大标题
###这是第三级，二级标题下面一级的小标题
####这是第四级，谨慎使用四级标题，尽量避免出现，保持层级的简单和防止出现过于复杂的章节。  

##列表
###无序列表(-/*/+跟着1+个空格，推荐用-)

```
- -开头
+ +开头
* *开头
```

效果：

- -开头
+ +开头
* *开头

###有序列表(数字跟着英文句点再跟1+个空格)

```
1. 正常1.开头，一个空格即可
2.   这里有多个（3个）空格也是可以的
2. 有序列表的数字不用在意顺序，这里还是2.也是可以的
3. 列表（有序或无序）的行之间
    最好有缩进（4个空格比较美观），
也可以没有缩进。

    这是第二段。列表多个段落的行首，必须有缩进。
行首出现数字加句点,需要使用\进行转义:
1987\. What a great season
```

效果：

1. 正常1.开头，一个空格即可
2.   这里有多个（3个）空格也是可以的
2. 有序列表的数字不用在意顺序，这里还是2.也是可以的
3. 列表（有序或无序）的行之间
    最好有缩进（4个空格比较美观），
也可以没有缩进。

    这是第二段。列表多个段落的行首，必须有缩进。
行首出现数字加句点,需要使用\进行转义:
1987\. What a great season

##文本样式

```
**2个\*包住的内容会加粗**  
*1个\*包住的内容会斜体*  
~~2个\~包住的内容会删除线~~   
```

效果：

**2个\*包住的内容会加粗**  
*1个\*包住的内容会斜体*  
~~2个\~包住的内容会删除线~~   

##水平线/分割线

多种方式表示分割线，推荐3个*表示，简单

```
星号*，3+个，中间可以或者不插入空格  
减号-，3+个，中间须插入1+个空格  
底线_，3+个，中间不能插入空格  
****
* * *
- --
___
```

效果：

星号*，3+个，中间可以或者不插入空格  
减号-，3+个，中间须插入1+个空格  
底线_，3+个，中间不能插入空格  
****
* * *
- --
___

##链接
###行内式
```
[我的网站](http://biaoqianwo.com)  
这是[MarkDown入门指南](http://www.jianshu.com/p/1e402922ee32/)  
![这是选填的alt](http://upload-images.jianshu.io/upload_images/807860-e6879dac34d09980.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "这是选填的title")  
```

效果：

[我的网站](http://biaoqianwo.com)  
这是[MarkDown入门指南](http://www.jianshu.com/p/1e402922ee32/)  
![这是选填的alt](http://upload-images.jianshu.io/upload_images/807860-e6879dac34d09980.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240 "这是选填的title")  

###参考式
```
I get 10 times more traffic from [Google] [1] than from [Yahoo] [2] or [MSN] [3].
[1]: http://google.com/   "Google Search"
[2]: http://search.yahoo.com/  "Yahoo Search"
[3]: http://search.msn.com/ (MSN Search)
```
或者
```
I get 10 times more traffic from [Google][] than from [Yahoo][] or [MSN][].
  [google]:http://google.com/        "Google"
  [yahoo]:  http://search.yahoo.com/
  [msn]:    http://search.msn.com/    "MSN Search"
```
链接内容定义的形式为：
- 方括号（前面至多三个空格来缩进），里面输入链接文字
- 接着一个冒号
- 接着0+个空格
- 接着链接的网址
- 接着选填的title，可以用双引号或括弧包着

效果：

I get 10 times more traffic from [Google][] than from [Yahoo][] or [MSN][].
  [google]:http://google.com/        "Google"
  [yahoo]:  http://search.yahoo.com/
  [msn]:    http://search.msn.com/    "MSN Search"

等同于行内式写法：

```
I get 10 times more traffic from [Google](http://google.com/ "Google") than from [Yahoo](http://search.yahoo.com/ "Yahoo Search") or [MSN](http://search.msn.com/ "MSN Search").
```

##引用
###一般引用
```
>以>开头的内容
>>多>就是引用的嵌套
```

效果：

>以>开头的内容
>>多>就是引用的嵌套

###多行引用
多行引用并不需要每一行都有>(首行必须有>，github上要求每行结尾2个空格，jianshu不要求)
```
>窗前明月光  
疑是地上霜  
举头望明月  
低头思故乡
```

效果：

>窗前明月光  
疑是地上霜  
举头望明月  
低头思故乡

##代码
###单行代码
```
`hello world`
```

效果：

`hello world`

```
``如果要在代码区段内插入反引号`，可以用多个反引号`包住``
```

效果：

``如果要在代码区段内插入反引号`，可以用多个反引号`包住``

###多行代码
````
```
<?php
function helloWorld(){
    echo "Hello world!";
}
```
````

效果：

```
<?php
function helloWorld(){
    echo "Hello world!"；
}
```

##反斜杠
以下这些符号前面加上反斜杠来帮助插入普通的符号：
```
\   反斜线 
`   反引号
*   星号
_   底线
{}  花括号
[]  方括号
()  括弧
#   井字号
+   加号
-   减号
.   英文句点
!   惊叹号
```

##表格

第一行是表头，第二行表示对齐，“-”2个+即可

```
|Id|Name|Price|
|:--|:--:|--:|
|1|白菜|1.5|
|2|胡萝卜|1|
|3|猪肉|15|
|左对齐|居中|右对齐|  
```

效果：

|Id|Name|Price|
|:--|:--:|--:|
|1|白菜|1.5|
|2|胡萝卜|1|
|3|猪肉|15|
|左对齐|居中|右对齐|  

##简写链接和邮件地址，用<>包住

```
<http://example.com/>  
<address@example.com>
```

效果：

<http://example.com/>  
<address@example.com>

##编辑器

推荐使用即时保存的[简书](http://jianshu.com)

##注意

github对于星号套星号，反引号套反引号的支持都不如jianshu。
通过上面的斜体和多行代码块，可以看出效果。[本文在github的地址](https://github.com/allen-li-webpower/markdown)。

##Enjoy it!
