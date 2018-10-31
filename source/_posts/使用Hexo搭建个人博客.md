---
title: 使用Hexo搭建个人博客
date: 2018-10-28 16:35:05
tags:
- Hexo
categories:
- 技术笔记
---

## GitHub环境准备

### 新建仓库
首先新建一个仓库，仓库名称一定要是：your github username.github.io的形式。
### 配置SSH Key

执行如下命令在本地生成SSH Key：
```
ssh-keygen -t rsa -C "Your GitHub register email address"
```

然后执行如下命令拷贝生成的key：

```
 # Copy the contents of the id_rsa.pub file to your clipboard
 pbcopy < ~/.ssh/id_rsa.pubs
```

最后将生产的Key添加到GitHub中。

## 安装Hexo等相关软件
###安装Node.js
通过[Node.js](https://nodejs.org/en/)官网下载并安装Node.js，用于下载Hexo等工具和插件。

###安装Hexo
执行如下命令：

```
npm install -g hexo-cli
```

## 搭建博客
### 初始化本地博客
首先新建一个文件夹，并在文件夹中执行如下命令。此时Hexo将会自动生成一些必须的文件。

```
hexo init
```

### 配置博客信息
博客的所有信息都是存储在_config.yml文件中，你可以根据需要进行配置。

