---
title: 浅谈新手Linux发行版的选择
date: 2017-03-21 19:08:58
tags:
  - Linux
categories:
  - Linux
---

# 前言

折腾的两年多的Linux，对于来说，我认为在这上面我还是一个新手。对于新手来说，如何选择一个Linux发行版，以及在什么地方使用Linux就是一个比较重要的问题了。虽然说的是对Linux发行版本的选择，其实准确的来说，应该是多主要的包管理器进行介绍，其他的在每个发行版本上都是大同小异的。

## 首要条件

学习Linux的话，中文的资料可能相对较少一些，找到的可能不是现在最新个版本的资料，所以得会使用各种搜索引擎，包括一些翻译软件。技术上的问题，能翻墙的尽量使用Google吧，不能的话使用Bing也是不错的选择，然后日常的话使用百度。

# 发行版介绍

在整个Linux发行版本中，有许多的发行版，主要的就那么几类：Redhat系、SUSE系列、ArchLinux系列以及Ubuntu系列。至于Gentoo和LSF我就不再进行讨论了，基本新手不回去碰的。

## Redhat系列

在这个系列中，主要有三个发行版本：RedHat Enterprise Linux、Fedora以及CentOS。主要都是使用yum作为包管理器，而在Fedora中正在测试使用DNF作为最新的包管理器。

对于新手来说，如果准备看《鸟哥的Linux私房菜》入门的话，应该会学习使用CentOS操作系统，这个系统是来源于对Redhat的源码的直接编译的结果，在Redhat收购CentOS社区后，这些就开始由开始由Redhat公司进行维护了。

Fedora的使用者相当于Redhat的企业版本的小白鼠，每隔6个月发布一个新的版本，许多新的技术都会先在Fedora上进行使用，然后在4个版本之后再发布一个新的Redhat的企业版。

使用的yum包管理器，感觉上就是各种插件，其图形化的前端，一直没用找到，并且对于软件包来说，没用deb的软件包多，使用的rpm打包方式也被人吐槽过，问题是我不知道哪里不好。。。

## SUSE系列

这个应该算是一个比较早的版本了，其主要的桌面环境是使用KDE，由此KDE的主要为维护者也是SUSE的开发者，在前年开始，SUSE和openSUSE社区开始发布了leap版本和tumbleweed的滚动版本。

如果说是日常使用，其有一个强大无比的管理工具——yast2，基本上在其他发行版本中遇到的一些配置问题，在openSUSE中基本就通过这个工具就解决了。虽然包管理器使用的是zypper，但是其打包的方式是rpm，所有会有大量的软件包来进行使用。

## Ubuntu和Debian

在许多推荐文中，都会发现推荐使用这两个发行版来进行学习，我认为这两个发行版也是入门Linux发行版比较好的选择。主要的原因是中文的社区大，虽然wiki没用ArchLinux的丰富，但是在日常的使用中，能在搜索引擎上使用中文轻松的查到许多的相关资料。

使用的包管理器是apt包管理器，使用起来应该是十分方便的，对于打包方式来说，deb那个近3万的软件包仓库加上Ubuntu自己的ppa社区源，基本上是不会没有软件使用这种说法的。

如果说是使用的话，我还是支持使用Windows和Mac作为日常的平台，在遇到开发问题的使用使用docker也能解决大部分的问题，其实目前来说，除非必要，不然主动去学习Linux平台的作为开发的可能性应该是十分低的。

## ArchLinux

这个应该是除了Gentoo和LFS外，自己可定制度最高的系统了，如果作为初学者，使用这个系统可能有点麻烦，但是如果跟着官方文档自己在虚拟机中搭建一边的话，就会对整个Linux体系有所了解了。

其使用pacman的包管理工具我个人认为有点简陋，但是十分好用，可能是我日常使用较少的原因把。其丰富的AUR源，在其中甚至能找到其他平台需要的东西和解决方案，可能只是需要自己在需要的平台上定制一下就行了。

# 结语

在几年前，我认为学习Linux是十分有必要的，但是现在，在有docker和vagrant的情况下，我的这个想法有所改变了。现在直接在物理机上搭建这个的过程已经没有必要了，如果在Windows上，有bash for Windows，在Mac上更加不用说。其实阻止我们日常使用Linux的最大原因是驱动问题，双显卡时候的安装Linux是十分麻烦的。对于日常来说，打字软件，QQ等聊天都不是一个日常使用的好平台，所以我的建议是在虚拟机中使用Linux，除非部署的时候使用Linux。
