---
title: 终于找到ubuntu下好用的五笔输入法iWubi,基于ibus
date: 2020-08-20 19:37:51
tags:
  - ubuntu
  - wubi
  - ibus
  - linux
  - 五笔
  - iWubi
---

# ubuntu下好用的五笔输入法iWubi,基于ibus

我在ubuntu上用过最好的五笔。
自从chrome突然有一个版本升级后，ubuntu自带的五笔[left shift]键在chrome下就不能切换中/英了，十分不习惯。
最近网上也有好多人在说这个，但一直没有好的解决方案，突然发现了这个，试用后太爽了！

### 原作者项目地址：<https://github.com/Honghe/iwubi>

![](/images/iwubi.gif)

python写的，安装的话没有deb安装包，不过安装超级简单，clone后：


``` sudo make install ```


目前没有设置选项，提示候选词为5个，采用是竖版提示。
我个人习惯多一点候选词和横版，所以fork了作者的项目，自己改了一下

![](/images/ch.png)

### 10个候选词＋横版提示，项目地址：<https://github.com/lizenghui/iwubi>
