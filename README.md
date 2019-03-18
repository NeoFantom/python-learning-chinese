# 中文Python学习指南

*2019年3月18日更新*

本文是一个中文的Python学习向导，力图尽可能简洁全面地介绍Python学习从入门到进阶的各方面。

## 安装与设置
### Python安装教程
本文这一部分尚未完成，请暂时先参考[Python3 环境搭建 | 菜鸟教程](http://www.runoob.com/python3/python3-install.html)。  
提示：在安装时勾选“Add to PATH”，可自动完成其中的设置环境变量步骤。

### [Anaconda](https://www.anaconda.com/)
Anaconda是一个自动包含了很多常用库、支持多版本Python安装、包含很多拓展功能的官方Python替代品。

## 工具
### IDE
IDE全称Integrated Develpment Envrionment即集成开发环境，是一类集编辑、编译、运行、测试等一体的软件工具。

#### [PyCharm](https://www.jetbrains.com/pycharm/)
本文推荐的Python IDE为JetBrains公司的PyCharm，这一IDE的优点在于它强大的代码补全、格式标准化、代码结构分析等功能。
#### 其他推荐IDE
[Sublime Text](https://www.sublimetext.com/)：轻巧通用的可拓展编辑器。  
[Jupyter Notebook](http://jupyter.org/)：置于浏览器中的轻量级编辑器，可编写LaTeX公式。
[Google Colab](https://colab.research.google.com/)：Google云上的基于Jupyter Notebook的在线IDE，其创立的主要目的是促进和方便机器学习的研究；可直接使用不需要配置，并可使用Google提供的免费CPU、GPU、TPU资源。（需要VPN）

## 库（library）、包（package）、模块（module）
Python的各种优秀的第三方包是Python编程简洁高效的重要原因之一，学会灵活地调包😜对于成为一个熟练的Python使用者至关重要。
### 使用Pip安装代码包
Pip是Python自带的包管理软件。确保Python安装时已被添加到系统环境变量PATH中，打开命令行（Windows系统需要以管理员运行）输入
```shell
pip ...
```
即可调用pip的各项功能。
以numpy为例，安装代码包的基本格式为
```shell
pip install numpy
```
然后等待下载并安装完毕即可。
### 基本格式
下文以numpy和numpy.array为例，列出了一些与导入包有关的基本代码。  
导入一个模块
```python
import numpy
```
导入一个模块并重命名
```python
import numpy as np
```
导入一个模块的一个变量或函数
```python
from numpy import array
```
导入一个模块的所有变量和函数
```python
from numpy import *
```
### [常用Python库简介](libraries.md)
此文列出了一些常用的Python库。
## 实用技巧
### help函数
使用help函数可以调出模块、类、函数、变量的说明文档，如
```python
import numpy as np

help(np.array)
```
即可调出numpy模块中array（数组）的说明文档。
## 学习方法
### 教程
#### [SoloLearn](https://www.sololearn.com/)
SoloLearn是一个在线学习编程的APP，有Android客户端、iOS客户端和网页版。  
  
SoloLearn有一个Python入门教程，以及一个关于Python常用的包NumPy的教程。使用网页版：[Python 3 Tutorial](https://www.sololearn.com/Course/Python/)。还可以在手机APP上，点击主页最左边的博士帽，查看所有可以学习的话题，包括Python 3和Python NumPy。

![SoloLearn Python 3 Tutorial](SoloLearn%20Python%203%20Tutorial.png)
  
SoloLearn还有一个Code Playground，无需安装任何环境，你就可以在线写一些简单的程序。你可以利用碎片时间在这里练习。

#### [Python3 教程 | 菜鸟教程](http://www.runoob.com/python3/python3-tutorial.html)
菜鸟教程是国内一个较好的编程基础入门教程网站，其Python教程分为Python 3基础教程和Python 3高级教程。其中Python 3基础教程内容较为完善适合初学者学习，也适合作为忘记特定功能写法时的参考；Python 3高级教程不需要专门学习，建议在需要使用到相关功能时结合实践学习。

#### Coursera [Python for Everybody Specialization](https://www.coursera.org/specializations/python)
这是Coursera网站首页推荐的一个Python编程课程集合，由美国密西根大学（University of Michigan）提供，包含五个课程，分别涉及编程基础、数据结构、Web数据访问、数据库、数据处理与可视化。你可以注册一个Coursera账号免费观看这些课程，同时也可以在上完课程后付费获取Coursera官方证书。

#### JetBrains [Python Edu](https://www.jetbrains.com/education/?fromMenu#lang=python&role=learner)
这是JetBrains开发的一个专门用于Python学习的软件插件，需要与上文提到的PyCharm配合使用。若已安装PyCharm，[安装EduTools Plugin](https://www.jetbrains.com/help/education/install-edutools-plugin.html?section=PyCharm)即可。

#### 其他视频
[[小甲鱼]零基础入门学习Python](https://www.bilibili.com/video/av4050443)是Bilibili上观看次数最多的一个Python教程系列视频。

### 编程练习
“纸上得来终觉浅，绝知此事要躬行。”编程练习是学习一门编程语言最重要的一个环节。

#### [LeetCode](https://leetcode.com/)
在这里向大家推荐一个编程练习网站LeetCode。  
注册账号并登陆后，在“Problems”一栏中便可看到此网站提供的所有问题，打开其中一个，在语言栏中选择“Python”，填写代码，点击“Submit Solution”即可提交，系统会自动检查你的代码是否正确。在正确完成大概10道题之后，你就能基本熟练掌握编程的基本操作。
