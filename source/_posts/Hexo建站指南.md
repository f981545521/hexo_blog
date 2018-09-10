---
title: Hexo建站指南
date: 2018-06-15 13:46:30
tags: hexo
---
### Hexo建站 


#### 安装前提
安装 Hexo 相当简单。然而在安装前，您必须检查电脑中是否已安装下列应用程序：
1. Node.js
2. Git

PS G:\hexo>  npm install -g hexo-cli
PS G:\hexo> hexo init D:\hexo
PS G:\hexo> npm install

> 参考[官方手册](https://hexo.io/zh-cn/docs/setup.html)

#### 主题
https://github.com/Haojen/hexo-theme-Claudia

#### Linux环境部署

1. 安装nodejs、npm
```
	[root@acyou ~]# yum install nodejs
	[root@acyou ~]# yum install npm
	[root@acyou ~]# node -v
	[root@acyou ~]# npm
```
2. 安装hexo
```
	[root@acyou ~]# npm config set strict-ssl false
	[root@acyou ~]# npm install -g hexo-cli
```


