---
author: lofei117
comments: true
date: 2013-01-22 07:00:56+00:00
layout: post
slug: design-of-class-configparser
title: ConfigParser类的设计
wordpress_id: 410
categories:
- MyRainmeter
tags:
- MyRainmeter
- 设计
---

一天天的不知道折腾什么，MyRainmeter弄到现在连ConfigParser类都还没搞定。

还是节奏没控制好啊。

ConfigParser类主要是一些针对initialization file的读写操作，其实是没什么太大的难度的， 利用windows的api就可以完成。

上个草图吧， 真是草图， 可能是由于自己的设计理念还不是很清晰，所以总感觉漏了点什么或者欠缺考虑的。

以后再慢慢改了， 完整的做下来以后才知道哪些地方不足， 才能完整的理解一个软件的具体开发设计。（虽然还是挺水的。）

[swf:/assets/swfs/ConfigParser-class-design.swf 600 500]

其实这个图前几天就画完了，然后一直琢磨着把类实现以后写一篇完整的，现在看来还是有好多东西没弄好。

从封装来说应该做到高度封装降低与其他模块的耦合性，但是实现的时候总是会想到其他的怎么和这个契合， 虽然说低耦合但还是有耦合的。

接口设计没设计好，模块与模块之间的关系没搞清楚。 导致的后果可能是那边弄完了回过头来这边改改。

坤比说的对， 怎么样把活分好分下去给手下的人做好，才是一个领导者该关心的，领导者不应该过于关心某件小事的实现细节。就像昨天看《楚汉传奇》里韩信被拜大将时对其余将军说的话， 大将军是管普通将军的， 不是冲锋陷阵带兵的， 如何运筹帷幄调度兵马才是他应该关心的。

昨天微博上看到某大神写的关于求职面试之类的云云， 看完了诸多感想，但是总归到底只有一个，自己的实力还不够，书看的还不够多。

慢慢来了。慢慢积攒代码量，慢慢提高自身修为。
