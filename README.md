# scss-demo
#### scss学习，[CSDN博客文章地址](https://blog.csdn.net/qq_41649879/article/details/84989306)

### 一、什么是SCSS？

SCSS是一种CSS预处理语言，在使用SCSS的过程中，可以使用编程的方式和思维。SCSS不能直接被浏览器解析，最后将其编译成真正的CSS语言，才会被浏览器所解析使用。

### 二、SCSS和SASS有什么区别？

SASS和SCSS其实是一种东西，二者主要有以下两点不同之处：

1. 文件扩展名不同。显而易见，SASS文件以“.sass”后缀为文件扩展名，而SCSS文件以“.scss”后缀为文件扩展名  
2. 语法书写方式不同。SASS是以严格的缩进式语法来书写，而SCSS和CSS文件类似，以“{ }”和“；”进行分隔

### 三、SASS的安装

sass基于Ruby语言开发而成，因此安装sass之前需要先安装Ruby，具体安装过程可参照开篇提到的课程Windows版、Mac版
安装完成后，在命令终端输入以下命令查看是否成功安装sass：

`sass -v`

通过以下命令对已安装的sass进行更新：

`gem update sass`

通过以下命令卸载sass：

`gem uninstall sass`

### 四、SASS的语法格式以及编译调试

#### 1. Sass语法格式

.css语法格式：
```
.container {
  width: 300px;
  height: 400px;
}
```
.scss语法格式：
```
$width: 300px;
$height: 400px;

.container {
  width: $width;
  height: $height;
}
```
.sass语法格式：
```
$width: 300px;
$height: 400px;

.container
  width: $width;
  height: $height;
```
#### 2. SASS编译

html中不能直接使用sass，因此需要将sass预先编译为css。sass的编译有多种方法：命令编译、GUI工具编译、自动化编译。

#### **1）sass命令编译**

即使用命令终端输入sass指令进行编译(使用watch功能进行实时监测)

（1）单文件编译：

sass --watch <要编译的Sass文件路径>/style.scss:<要输出CSS文件路径>/style.css

（2）多文件编译：

sass --watch <要编译的含.Sass/.scss文件的文件夹路径>:<要输出CSS文件路径>



