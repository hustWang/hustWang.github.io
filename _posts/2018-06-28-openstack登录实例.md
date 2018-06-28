---
layout: post
title: openstack登录实例
categories: openstack
description: openstack，镜像
keywords: root，注入
---

- 新建镜像实例时对实例的root密码自定义

  ```
  1. 对于控制节点，修改nova的配置
     /etc/nova/nova.conf
     将inject_password改为true 。
     重启nova服务：systemctl restart openstack-nova-*
     
  2. 在创建虚拟机时注入脚本，以网页上操作为例
     1）在创建实例的 配置 项中注入脚本
        #!/bin/sh
        passwd root<<EOF
        name
        name
        EOF
      2）勾选配置驱动
      3）在实例启动后，等待控制台显示 实例名称 login：，则说明注入成功。 
  ```
