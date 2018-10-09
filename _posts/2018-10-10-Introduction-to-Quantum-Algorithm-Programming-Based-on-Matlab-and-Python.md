---
layout: post
title:  "基于Matlab和Python的量子算法编程简介"
categories: Quantum Programming 
tags:  Algorithm Matlab Python
author: litong
---

* content
{:toc}

## 1、概述：
量子编程和传统计算机编程一样，都是是组装指令序列的过程。不过通过量子编程之后，产生的源代码称为量子程序。在做量子编程时，注意一下几个概念：

### 1.1、量子指令集
量子指令集用于将量子算法转换为可以在量子处理器上执行的物理指令，这些特定的指令是能够在量子计算机上运行的（如离子阱，超导量子计算机，光量子计算机等）。如，Quil、OpenQASM指令集。

### 1.2、量子软件开发工具包
量子软件开发工具包提供了创建和操作量子程序的工具集，它们还提供了模拟量子程序的API，或基于云平台的量子计算机运行量子程序的接口。

#### 1.2.1、基于访问量子处理器的量子软件开发工具包
现在已经有一些量子软件开发工具包，可以在真实的量子计算机上或量子模拟器上运行量子电路。如：
ProjectQ，由苏黎世联邦理工学院理论物理研究所启动的量子计算开源软件框架，它使用Python编程语言来创建和操纵量子电路。在基于自己的模拟器运行，以获得量子程序运行的结果。或将作业发送到IBM量子设备来获得结果。
Qiskit，由IBM开发的一个开源项目。量子电路使用Python，Swift或Java创建和操作。在基于IBM提供的模拟器或云平台的量子计算机上，用户可以在自己的电脑上运行量子程序，以获得量子程序运行的结果。
当然，量子软件开发工具包还有ProjectQ，Forest等。

#### 1.2.2、基于模拟器的量子软件开发工具包
ProjectQ，Qiskit都有自己的模拟器。

#### 1.2.3、量子信息工具包
Quantum Information Toolkit（QIT）是一个免费的开源数字工具包，用于各种量子信息和量子计算相关的目的，......。

## 2、matlab编程介绍（QIT）：







```js
/usr/share/applications
```

## 解压

这里我将pycharm下载并解压到了/home/snakeson/developer文件夹下

这里的pycharm.sh是批处理执行文件，prcharm.png是快捷方式图标

## 终端打开

使用Ubuntu终端进行打开：
方法一（使用vim）：
```js
sudo vi  /usr/share/applications/pycharm.desktop
```

方法二（使用gedit）：
	
```js
sudo gedit  /usr/share/applications/pycharm.desktop
```





然后就会弹出一个新框：
## 张贴
我们将下面的内容贴上去：
```js

[Desktop Entry]
Type=Application
Name=Pycharm
GenericName=Pycharm3
Comment=Pycharm3:The Python IDE
Exec="/home/snakeson/developer/pycharm-community-2017.2.3/bin/pycharm.sh" %f
Icon=/home/snakeson/developer/pycharm-community-2017.2.3/bin/pycharm.png
Terminal=pycharm
Categories=Pycharm;

```
---
注意一定要将Desktop Entry复制进去，也就是上面的全部都要复制进去，这里我们需要替换掉两个地方：**Exec="xx"**和**Icon=**,这里要替换掉我们的pycharm解压的目录，当然了，我已经替换好了，如果你的目录跟我的目录不一样的话，你得把路径给换了，不管你是pycharm2017还是pycharm2016,，例如Comment什么的都不要改变，只变上面提到的两个路径就可以了。


## 添加可执行权限
```js
sudo chmod +x /usr/share/applications/pycharm.desktop
```

## 拷贝到桌面
```js
将/usr/share/applications/pycharm.desktop文件拷贝到桌面，双击即可运行。
```