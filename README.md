# ROS Melodic Install
### This is about ROS for Windows and Ubuntu(install tutorials and problems solution)

Read this in other languages: [English](https://github.com/Harryjin0326/ROS-Install/blob/master/README.md), [简体中文](https://github.com/Harryjin0326/ROS-Install/blob/master/README-zh.md)

#### Table of contents

## 1.Ubuntu install of ROS Melodic
### 1.1 Configure your Ubuntu repositories
Setup your computer to accept software from packages.ros.org.
```java
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```
Or the accept software from China
```java
sudo sh -c '. /etc/lsb-release && echo "deb http://mirrors.ustc.edu.cn/ros/ubuntu/ $DISTRIB_CODENAME main" > /etc/apt/sources.list.d/ros-latest.list'
```
