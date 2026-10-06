---
title: 我的第一篇博客
subtitle: 从重新搭建博客到重新出发
date: 2026-04-29T20:10:59+08:00
slug: 0d54685
draft: false
author:
  name: 二哈
  link: https://github.com/GrumpyTeddy
  email: moleyunfei@gmail.com
  avatar: /images/avatar.jpg
description: mac配置教程
keywords:
  - hugo
  - blog
  - mac
  - setting
  - 
comment: true
weight: 0
tags:
  - hugo
  - setting
  - blog
categories:
  - graphics
hiddenFromHomePage: false
hiddenFromSearch: false
hiddenFromRelated: false
hiddenFromFeed: false
summary: 自己mac的到手配置教程，欢迎大家补充。
featuredImagePreview:
featuredImage:
password:
message:
repost:
  enable: false
  url:

# See details front matter: https://fixit.lruihao.cn/documentation/content-management/introduction/#front-matter
---

<!--more-->

## mac到手配置日记

为了保持mac的简洁性以及高效率，易用性，翻阅了众多资料以及询问了朋友，最终配置好了自己的mac，但是目前也还有很多没修改，欢迎大家多留言

### 基础设置

0. 首先需要了解的内容
   1️⃣ mac的文件管理与windows逻辑不同，可能需要习惯。
   2️⃣ mac安装软件时，有下载好dmg打开双击，下载好dmg拖移，具体安装流程都有说明，很简单。
   3️⃣ 建议使用uv管理python环境，保持环境简洁性

1. 打开三指拖移(强烈建议打开 很重要，很方便的一个设置)：
   设置-辅助功能-指针控制-拖移样式改为三指拖移
   直接设置搜索拖移样式-点开改为三指拖移

2. 终端配置
   如果个人喜好shell 可以不配置，但是为了更高的可用性，强烈建议安装oh-my-zsh插件，直接官网搜索即可
   同时官网也有对应的主题，下载好oh-my-zsh之后,使用 nano ～/.zshrc 找到对应名称叫zsh theme的，修改引号里的内容即可。
   nano使用：可以查看介绍 我这里介绍几个比较简单的
   nano进入之后 按control+w 即可展开搜索 输入要搜索的内容回车即可跳转

具体插件介绍：可以在github搜索ohmyzsh或者官网，找到**仓库里的plugins**文件夹，点进入点进去查看每个插件的作用
插件安装：同样 nano 搜索到 plugins=() 默认应该是带git的 直接往() 里添加内容即可，然后使用source ~/.zshrc激活

目前我使用的一些插件
plugins=(
  git git的别名
  docker 为docker添加了自动补全和命令别名，具体别名在github仓库即可查看
  docker-compose。作用同上，别名也是用同样的方式
  tmux.  同样也是tmux的别名
  shell-proxy 作用是为终端添加代理，首先需要的是clash、v2ray等 具体方法查看GitHub
  history 别名：history原命令的作用是打印你的历史命令
  extract 解压文件 但是没试过
  universalarchive. 打包 没尝试过
  rsync 同步 复制 传输文件 也是多了一些别名
  aliase 用于查询别名 als git 等等 具体见github
  alias-finder 不使用别名时 提示你使用别名
  fzf. 用户模糊搜索 文件、目录、指令等
  fzf-tab. 
  zsh-autosuggestions.  弹出提示时 按右方向键即可补全
  zsh-syntax-highlighting 用颜色提示当前命令是否正确
)
最后三个 faf tab zsh- 三个需要前往github pull
有些比较小的代码 如果不想打开vscode 可以用vim
下载lazyvim插件包即可


3. 建议使用homebrew来管理安装软件，而不是使用应用商店store