---
title:  Run ROS Project
tags:
  - ROS
  - qtc_plugin
  - Tutorial
typora-root-url:  ..
---

使用Qt Creator创建ROS工程

编译运行ROS工程

<!--more-->

## ROS Terminals

Qtc pulgin安装之后会自动增加一个`ROS Terminals`窗口方便运行ros各个节点。默认情况下`ROS Terminals`是没有打开的需要手动选择下。
<img src="/images/11.png" alt="01" style="zoom: 67%;" />

选择之后，需要点击左上角的新建Terminal按钮（因为是灰色的，不容易注意到）来打开一个terminal。反而**+，-**是用来调节字体大小的，是有点歧义感觉。

## catkin编译系统下ROS的工作空间结构

<img src="/images/13.png" alt="01" style="zoom: 67%;" />

## 新建一个ROS Package

1. 在src文件下右键选择`Add New...`

<img src="/images/12.png" alt="01" style="zoom: 67%;" />

<img src="/images/14.png" alt="01" style="zoom: 67%;" />

2. 填写创建包的信息

<img src="/images/15.png" alt="01" style="zoom: 67%;" />

<img src="/images/16.png" alt="01" style="zoom: 67%;" />

注意：

- **Name**和**Path**这两个必须填写。其他部分根据需要填写，即使没有填写后续也可以修改文件来增删。
- 左侧项目部分有可能不显示新创建的package，实际上是已经创建了对应的文件。这种情况下重启下Qt Creator就行。

至此在Qt Creator中创建新的package就成功了。

参考：

- https://ros-qtc-plugin.readthedocs.io/en/latest/_source/Import-ROS-Workspace.html
- [https://github.com/huchunxu/ros_21_tutorials/blob/e52d8a78d46ec90b7367e461ab157668eb666e45/docs/slides/%E5%8F%A4%E6%9C%88%20%C2%B7%20ROS%E5%85%A5%E9%97%A821%E8%AE%B2_9.%E5%88%9B%E5%BB%BA%E5%B7%A5%E4%BD%9C%E7%A9%BA%E9%97%B4%E4%B8%8E%E5%8A%9F%E8%83%BD%E5%8C%85.pdf](https://github.com/huchunxu/ros_21_tutorials/blob/e52d8a78d46ec90b7367e461ab157668eb666e45/docs/slides/古月 · ROS入门21讲_9.创建工作空间与功能包.pdf)