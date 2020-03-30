---
title:  Import ROS Project
tags:
  - ROS
  - qtc_plugin
  - Tutorial
typora-root-url:  ..
---

使用Qt Creator导入已有ROS的worksapce。如果没有ROS workspace情况下按照下面步骤操作。默认情况下，只是创建了`catkin_ws.workspace`这个文件，没有标准的`catkin_init_workspace`命令生成的文件。还是需要**catkin_init_workspace**命令用来创建空间文件。

<!--more-->

## Step 0

创建一个工作空间

```shell
$mkdir -p ~/catkin_ws/src
$cd ~/catkin_ws/src
$catkin_init_workspace
```

编译工作空间

```shell
$cd ~/catkin_ws
$catkin_make
```

设置环境变量

```shell
$source devel/setup.bash
```

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

至此导入ROS的工作空间工程就成功了。

参考：

- https://ros-qtc-plugin.readthedocs.io/en/latest/_source/Import-ROS-Workspace.html
- https://github.com/huchunxu/ros_21_tutorials/blob/e52d8a78d46ec90b7367e461ab157668eb666e45/docs/slides/古月 · ROS入门21讲_9.创建工作空间与功能包.pdf