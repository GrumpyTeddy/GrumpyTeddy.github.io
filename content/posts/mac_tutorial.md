---
title: mac配置教程
date: 2026-10-07T00:10:59+08:00
slug: 0d54685
draft: false
author:
  name: 二哈
  link: https://github.com/GrumpyTeddy
  email: moleyunfei@gmail.com
  avatar: /images/avatar.jpg
description: 自己 Mac 的到手配置教程，欢迎大家补充。
keywords:
  - mac
  - setting
comment: true
tags:
  - mac
  - setting
categories:
  - setting
summary: 自己 Mac 的到手配置教程，欢迎大家补充。
---

<!--more-->

## Mac 到手配置日记

为了保持 Mac 的简洁性、高效率和易用性，翻阅了众多资料以及询问了朋友，最终配置好了自己的 Mac。目前也还有很多没修改，欢迎大家多留言。

### 基础设置

#### 0. 首先需要了解的内容

- 1️⃣ Mac 的文件管理与 Windows 逻辑不同，可能需要习惯。
- 2️⃣ Mac 安装软件时，有下载好 dmg 打开双击、下载好 dmg 拖移等方式，具体安装流程都有说明，很简单。
- 3️⃣ 建议使用 `uv` 管理 Python 环境，保持环境简洁性。

#### 1. 打开三指拖移（强烈建议）

{{< admonition type=tip title="很重要，很方便的一个设置！" open=true >}}

两种方式任选其一：

- **路径方式**：设置 → 辅助功能 → 指针控制 → 拖移样式 → 改为三指拖移
- **搜索方式**：设置里直接搜索"拖移样式" → 点开改为三指拖移

{{< /admonition >}}

#### 2. 终端配置

如果个人喜好原生 shell 可以不配置，但为了更高的可用性，**强烈建议安装 [oh-my-zsh](https://ohmyz.sh/)**，直接官网搜索即可。

官网也有对应的主题。下载好 oh-my-zsh 之后，使用 `nano ~/.zshrc` 找到名称叫 `ZSH_THEME` 的，修改引号里的内容即可。

**nano 简单操作：**

- 进入之后按 `Ctrl + W` 展开搜索，输入内容回车即可跳转

**插件介绍：**

具体可以在 GitHub 搜索 `ohmyzsh` 或官网，找到**仓库里的 `plugins`** 文件夹，点进去查看每个插件的作用。

**插件安装：**

同样用 `nano` 搜索到 `plugins=()`（默认应该是带 git 的），直接往 `()` 里添加内容即可，然后使用：

```bash
source ~/.zshrc
```

来激活配置。

目前我使用的一些插件：

```bash
plugins=(
  git                 # git 的别名
  docker              # 为 docker 添加自动补全和命令别名，具体别名在 github 仓库查看
  docker-compose      # 作用同上
  tmux                # tmux 的别名
  shell-proxy         # 为终端添加代理，需配合 clash/v2ray 等，具体方法查看 GitHub
  history             # 别名：history 原命令是打印历史命令
  extract             # 解压文件（还没试过）
  universalarchive    # 打包（还没试过）
  rsync               # 同步、复制、传输文件，多了一些别名
  aliases             # 用于查询别名 als git 等等，具体见 github
  alias-finder        # 不使用别名时提示你使用别名
  fzf                 # 模糊搜索文件、目录、指令等
  fzf-tab             # fzf 的 tab 补全增强
  zsh-autosuggestions # 弹出提示时，按右方向键即可补全
  zsh-syntax-highlighting # 用颜色提示当前命令是否正确
)
```

{{< admonition type=warning title="注意" open=false >}}

最后三个（`fzf`、`fzf-tab`、`zsh-autosuggestions`、`zsh-syntax-highlighting`）需要前往 GitHub 手动 clone 安装，不在 oh-my-zsh 内置仓库里。

{{< /admonition >}}

有些比较小的代码，如果不想打开 VSCode，可以用 vim。下载 LazyVim 插件包即可。

#### 3. 软件安装

建议使用 **Homebrew** 来管理安装软件，而不是使用应用商店。