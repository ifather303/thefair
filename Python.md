# Python

## 基础

1. 程序执行的方式：编译VS解释

* 编译：将源代码一次性转换成目标代码的过程（翻译）==》静态语言
* 解释：将源代码逐条转换成目标代码并同时执行的过程（同声传译）==》脚本语言

2. 程序基本编写方法：IPO

* I：Input：程序输入
* P：Process：程序处理（算法）
* O：Output：程序输出 

3. 编程解决问题的步骤

* 分析问题
* 划分边界
* 设计算法
* 编写程序
* 调试测试
* 升级维护

## 前期准备

### 安装Python



### 安装集成开发环境（IDE）

#### 编译器

[Sublimse Text3](https://www.sublimetext.com/3)

#### 配置

安装[Package Control](https://packagecontrol.io/installation),重启软件，点击 菜单上的“Preferences” -> “Package Control”，然后选择 Package Control：Install Package

1. 汉化

   ChineseLocalizations

2. 配置Python环境

   SublimeREPL（类似于Python自带的IDLE）

   设置快捷键

   打开 preferences   ->  key bindings 复制下列代码，保存即可(下列快捷键是指安F5执行程序)

   ```
   {   
   "keys":["f5"],  
   "caption": "SublimeREPL: Python - RUN current file",  
   "command": "run_existing_window_command", "args": {"id": "repl_python_run",  
   "file": "config/Python/Main.sublime-menu"}  
   }
   ```


注释

* 单行注释：以#开头
* 多行注释：以"""作为开头以及结尾

变量

* 定义：用来保存和表示数据的占位符号
* 命名
  * 元素：字母，数字，下划线，汉字
  * 注意：大小写敏感，首字符不能是数字，或保留字（关键字）
* 赋值：以等号(=)赋值

## 数据类型

程序设计语言不允许存在语法歧义，所以需要定义数据形式

#### 字符串

##### 定义

由0个或多个字符串组成的**有序**字符序列

##### 表示

由一对单引号('')或者一对双引号("")表示

##### 索引

###### 定义

返回字符串中特定个数的字符

###### 表示

<字符串>[M]

* 正向递增序号：从0开始
* 负向递减序号：从-1开始

##### 切片

###### 定义

返回字符串中特定个数的字符

###### 表示

<字符串>[M:N] 不取N对应的字符

#### 列表

## 语句与函数

### 语句

#### 种类

* 赋值语句

* 分支语句：由判断条件决定的程序运行的语句

  每个保留字所在行最后存在一个冒号(:)

### 函数

#### 输入函数

##### input函数

#### 输出函数

##### print函数

###### 表现形式

###### 格式化

#### 其他函数

##### eval函数(评估函数 )

###### 定义

去掉参数最外层引号并执行余下语句的函数

## Python库

库Library=包Package=模块Module

### 标准库

随解释器直接安装到电脑的功能模块

#### 引用

* 标准引用

import<库名>

<库名>.<函数名>(<函数参数>)

* 简易引用(一)：容易出现函数名重复的情况

from <库名> import

from <库名> import *

<函数名>(<函数参数>)

* 简易引用(二)：不容易出现函数名重复的情况

from <库名> import as <库别名>

<库别名>.<函数名>(<函数参数>)

### 第三方库

需要经过安装才能使用的功能模块

