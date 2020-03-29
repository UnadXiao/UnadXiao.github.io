---
title:  Build ROS Project
tags:
  - ROS
  - qtc_plugin
  - Tutorial
typora-root-url:  ..
---

使用Qt Creator创建ROS工程

<!--more-->

## Step 1

1. 打开Qt Creator
2. 在菜单`文件`选项，选择`新建文件或项目`项目  **其他项目 -》 ROS Workspace**
<img src="/images/07.png" alt="01" style="zoom: 67%;" />

## Step 2

1. 填写工作空间信息

<img src="/images/08.png" alt="01" style="zoom: 67%;" />

| 项             | 描述                            |
| -------------- | ------------------------------- |
| Name           | 工程名字                        |
| Distribution   | ROS版本 (indigo, kinetic, etc.) |
| Build System   | 所需的构建系统。                |
| Workspace Path | 工作空间文件路径                |

2. 下一步，完成

<img src="/images/09.png" alt="01" style="zoom: 67%;" />

## Step 3

默认情况下，Qt Creator会隐藏空文件路夹（新创建的内容是空的）。将**Hide Empty Directories**选项去掉就可以了。

<img src="/images/10.png" alt="01" style="zoom: 67%;" />

至此一个ROS的工作空间工程就创建成功了。

参考：

- https://ros-qtc-plugin.readthedocs.io/en/latest/_source/Import-ROS-Workspace.html