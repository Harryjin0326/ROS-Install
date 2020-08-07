# ROS Melodic Install
### This is about ROS for Windows and Ubuntu(install tutorials and problems solution)

Read this in other languages: [English](https://github.com/Harryjin0326/ROS-Install/blob/master/README.md), [简体中文](https://github.com/Harryjin0326/ROS-Install/blob/master/README-zh.md)

#### Table of contents

## 1.Ubuntu install of ROS Melodic
### 1.1 Configure your Ubuntu repositories
Configure your Ubuntu repositories to allow "restricted," "universe," and "multiverse."
### 1.2 Setup your sources.list
Setup your computer to accept software from packages.ros.org.
```java
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```
Or the mirrors from China
```java
sudo sh -c '. /etc/lsb-release && echo "deb http://mirrors.ustc.edu.cn/ros/ubuntu/ $DISTRIB_CODENAME main" > /etc/apt/sources.list.d/ros-latest.list'
```
### 1.3 Set up your keys
```java
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```
### 1.4 Installation
First, make sure your Debian package index is up-to-date:
```java
sudo apt-get update
```
There are many different libraries and tools in ROS. We provided four default configurations to get you started. You can also install ROS packages individually.
#### Desktop-Full(Recommended): ROS, rqt, rviz, robot-generic libraries, 2D/3D simulators and 2D/3D perception
```java 
sudo apt install ros-melodic-desktop-full
```
