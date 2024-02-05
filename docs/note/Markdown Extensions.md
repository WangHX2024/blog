# Markdown 拓展语法
## 第一讲：
隐藏页面下方“上一页/下一页栏

代码：
```
---
hide:
    - footer    
---
```

## 第二讲：告诫语法
### 2.1 告诫语法
!!! note
    
    这是告诫文本，开头缩进4个空格。

代码：
```
!!! note
    
    这是告诫文本，开头缩进4个空格。
```

### 2.2 告诫语法（自定义标题）
!!! note "告诫标题"
    
    这是告诫文本，开头缩进4个空格。

代码：
```
!!! note "告诫标题"
    
    这是告诫文本，开头缩进4个空格。
```

### 2.3 告诫语法（无标题）
!!! note ""
    
    这是告诫文本，开头缩进4个空格，并且此语法不适用于可折叠块。

代码：
```
!!! note ""
    
    这是告诫文本，开头缩进4个空格，并且此语法不适用于可折叠块。
```

### 2.4 告诫语法（可折叠，默认状态为折叠）
??? note

    这是告诫文本，开头缩进4个空格。

代码：
```
??? note

    这是告诫文本，开头缩进4个空格。
```

### 2.5 告诫语法（可折叠，默认状态为展开）
???+ note

    这是告诫文本，开头缩进4个空格。

代码：
```
???+ note

    这是告诫文本，开头缩进4个空格。
```

### 2.6 类型限定符
以上的note，可替换为abstract、info、tip、success、question、warning、failure、danger、bug、example、quote

## 第三讲：注释语法
这是一段需要注释(1)的文本(2)。注释可应用在文本、告诫、内容选项卡等多处，也可以嵌套使用。{.annotate}

1.  这是(1)处注释的内容。
2.  这是(2)处注释的内容。

代码：
```
这是一段需要注释(1)的文本(2)。注释可应用在文本、告诫、内容选项卡等多处，也可以嵌套使用。{.annotate}

1.  这是(1)处注释的内容。
2.  这是(2)处注释的内容。
```

## 第四讲：代码块
``` cpp title="example.cpp" linenums="1" hl_lines="2 3"
//这是一段C++代码，被包含三个反引号`（在键盘左上角）的两行单独括起来，并且可以在第一行后添加语言简码、代码块标题、行号（本例行号从1开始）、突出显示特定行行的行号（本例为2、3行）
#include<iostream>
using namespace std;
int main()
{
    ;
}
```

代码：
```
``` cpp title="example.cpp" linenums="1" hl_lines="2 3"
//这是一段C++代码，被包含三个反引号`（在键盘左上角）的两行单独括起来，并且可以在第一行后添加语言简码、代码块标题、行号（本例行号从1开始）、突出显示特定行行的行号（本例为2、3行）
#include<iostream>
using namespace std;
int main()
{
    ;
}
```

## 第五讲：内容选项卡
内容选项卡中可以添加代码块等，内容选项卡也可以被嵌入告诫等块。

=== "选项1"
    选项1的内容。
=== "选项2"
    选项2的内容。

代码：
```
=== "选项1"
    选项1的内容。
=== "选项2"
    选项2的内容。
```

## 第六讲：表
下表是左对齐的。

更改为居中：分割线左右都加冒号。

更改为右对齐：分割线右侧加冒号。

| Method   | Description     |
| :------- | :---------------|
| GET      | Fetch resource  |
| PUT      | Update resource |
| DELETE   | Delete resource |

代码:
```
| Method   | Description     |
| :------- | :---------------|
| GET      | Fetch resource  |
| PUT      | Update resource |
| DELETE   | Delete resource |
```

## 第七讲：脚注
这是一段需要插入脚注的文字[^1]。

[^1]:
    这是脚注内容。

代码：
```
这是一段需要插入脚注的文字[^1]。
[^1]:
    这是脚注内容。
```

## 第八讲：网格
### 8.1 List语法

<div class="grid cards" markdown>

-   :material-clock-fast:{ .lg .middle } 网格1

    ---

    内容1

    [:octicons-arrow-right-24: 链接1](#)

-   :fontawesome-brands-markdown:{ .lg .middle } 网格2

    ---

    内容2

    [:octicons-arrow-right-24: 链接2](#)

</div>

代码：
```
<div class="grid cards" markdown>

-   :material-clock-fast:{ .lg .middle } 网格1

    ---

    内容1

    [:octicons-arrow-right-24: 链接1](#)

-   :fontawesome-brands-markdown:{ .lg .middle } 网格2

    ---

    内容2

    [:octicons-arrow-right-24: 链接2](#)

</div>
```

### 8.2 通用网格
通用网格允许在网格中排列任意块元素，包括告诫、代码块、内容选项卡等。例如：

```
<div class="grid" markdown>

=== "Unordered list"

    * Sed sagittis eleifend rutrum
    * Donec vitae suscipit est
    * Nulla tempor lobortis orci

=== "Ordered list"

    1. Sed sagittis eleifend rutrum
    2. Donec vitae suscipit est
    3. Nulla tempor lobortis orci

``` title="Content tabs"
=== "Unordered list"

    * Sed sagittis eleifend rutrum
    * Donec vitae suscipit est
    * Nulla tempor lobortis orci

=== "Ordered list"

    1. Sed sagittis eleifend rutrum
    2. Donec vitae suscipit est
    3. Nulla tempor lobortis orci
```

</div>
```

## 第九讲：图标与表情
图标搜索：https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/#search

使用：将表情符号的短代码放在两个冒号之间:smile:

代码：`:smile:`