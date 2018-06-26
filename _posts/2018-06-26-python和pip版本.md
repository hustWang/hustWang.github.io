---
layout: post
title: python和pip版本
categories: python
description: python，pip
keywords: python，pip
---

- 为python和python3安装pip

  ```
  sudo apt-get install python-pip
  sudo apt-get install python3-pip

  卸载：
  sudo apt-get remove

  查看版本：
  python --version  pip --version
  ```

- 更改ubuntu默认python版本

  ```
  安装ubuntu过程有可能同时为你提供多个可用的 Python 版本，因此系统中会存在多个 Python 的可执行二进制文件。一般Ubuntu默认的Python版本都为2.x。
  1. 查看ubuntu中的所有python版本
     ls /usr/bin/python*
  2. 默认的python版本
     python --version
  ```
  - 基于用户修改python版本

    ```
    1. 打开该用户的 ~/.bashrc文件，添加新的别名信息来修改默认使用的 Python 版本
       alias python='/usr/bin/python3.4'
    2. 重新登录或者重新加载 .bashrc 文件，使操作生效。
       . ~/.bashrc
    ```