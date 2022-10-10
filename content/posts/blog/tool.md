---
title: "tool"
date: 2022-05-05T00:18:23+08:00
lastmod: 2022-05-05T00:18:23+08:00
author: ["Zain"]
keywords: 
- 
categories: 
- 
tags: 
- blog
- tool
description: ""  #描述
weight:  # 输入1可以顶置文章，用来给文章展示排序，不填就默认按时间排序
slug: ""
draft: false # 是否为草稿
comments: true
reward: true # 打赏
mermaid: true #是否开启mermaid
showToc: true # 显示目录
TocOpen: true # 自动展开目录
hidemeta: false # 是否隐藏文章的元信息，如发布日期、作者等
disableShare: true # 底部不显示分享栏
showbreadcrumbs: true #顶部显示路径
cover:
    image: "" #图片路径例如：posts/tech/123/123.png
    caption: "" #图片底部描述
    alt: ""
    relative: false
---


# WSL

## 安装ubuntu20.04

安装到非系统盘目录，下载离线安装包，复制到想要安装的目录下，解压，以管理员身份运行ubuntu2004.exe

## 卸载wsl

```sh
wslconfig /l
# 从列表中选择要卸载的发行版（例如Ubuntu）并键入命令
wslconfig /u Ubuntu
```
参考链接：[WSL系列操作：安装，卸载](https://blog.csdn.net/zhangpeterx/article/details/97616268
)

## 设置wsl
```sh
# 更改默认root用户登录
ubuntu1804.exe config --default-user root
# 更改默认登陆目录
# list 中 Ubuntu-20.04 条目中添加
"startingDirectory": "//wsl$/Ubuntu-20.04"

# 以管理员权限运行cmd
# 停止
net stop LxssManager  
# 启动
net start LxssManager 
```



# PowerShell

```sh
winget search Microsoft.PowerShell
winget install Microsoft.PowerShell
```
参考链接：
- [Windows Powershell和Windows Terminal的区别](https://blog.csdn.net/The_Time_Runner/article/details/106038222)


- [安装和设置 Windows 终端](https://docs.microsoft.com/zh-cn/windows/terminal/get-started)


# windows 包管理工具

## winget 官方推出

```sh
# 使用 WinGet 安装一遍
winget install postman
winget search postman

# 卸载，再用 Scoop 安装一遍
scoop install postman
```

## choro


##  vcpkg
[Get started with vcpkg](https://vcpkg.io/en/getting-started.html)

## cget
https://cget.readthedocs.io/en/latest/#

[开源库集成器Vcpkg全教程](https://blog.csdn.net/cjmqas/article/details/79282847)

##  Scoop 


#  图床


 https://blog.csdn.net/qq_44314954/article/details/122951033


# vscode

## vscode 上传图片

```sh
# 上传剪贴板中的图片到服务器。
ctrl + alt + u
# 打开文件浏览器选择图片上传。
ctrl + alt + e

```
- https://www.jianshu.com/p/868b3a2028f8
https://zhuanlan.zhihu.com/p/131584831