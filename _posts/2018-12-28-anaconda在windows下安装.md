---
layout: post
title: anaconda在windows下安装
categories: python
description: anaconda，python
keywords: anaconda，python
---

- 安装

  ```
  1. 下载：https://www.anaconda.com/download/
  2. 到 Advanced Options 这步时，两个选项都勾选，到安装完成
  ```

- 使用

  ```
  1. 安装好anaconda3后，在将会有一个Anaconda Navigator 的应用，打开并运行它，选中Enviroments这个选项。
  2. 选择create选项，创建自定义的python环境，如python3.5
  3. 如下图，右侧为py35环境对应的已安装的相关包和版本信息。
  4. 点击py35后的执行按钮，选择open Terminal，打开py35环境对应的终端，切换到xxx.whl包对应的目录，即可进行相应python包的安装。其余环境同理。以此解决不同python版本下需要安装python包的问题。 
  ```

  ![anaconda](E:\文档2017_18\OpenStack\VMI\新学期\20181113+\20190102\anaconda.PNG)