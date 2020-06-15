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

PS G:\hexo> npm install -g hexo-cli
PS G:\hexo> hexo init D:\hexo
PS G:\hexo> npm install

> 参考[官方手册](https://hexo.io/zh-cn/docs/setup.html)
> 参考[操作命令手册](https://hexo.io/zh-cn/docs/commands)

#### 主题
https://github.com/Haojen/hexo-theme-Claudia

#### Linux环境部署

1. 安装nodejs、npm
 - （弃用）
```
	[root@acyou ~]# yum install nodejs
	[root@acyou ~]# yum install npm
	[root@acyou ~]# node -v
	[root@acyou ~]# npm
```
 - （推荐）注意用户名路径
 ```
	[root@acyou nodejs]# wget http://cdn.npm.taobao.org/dist/node/v10.8.0/node-v10.8.0-linux-x64.tar.xz
	[root@acyou nodejs]# xz -d node-v10.8.0-linux-x64.tar.xz
	[root@acyou nodejs]# tar -xvf node-v10.8.0-linux-x64.tar 
	[root@acyou hexo_blog]# ln -s /youfang/nodejs/node-v10.8.0-linux-x64/bin/node /usr/local/bin/
	[root@acyou hexo_blog]# ln -s /youfang/nodejs/node-v10.8.0-linux-x64/bin/npm /usr/local/bin/
 ```
> 如不生效请重启服务器
2. 安装hexo
```
	[root@acyou ~]# npm config set strict-ssl false
	[root@acyou ~]# npm install -g hexo-cli
```
3. 部署
```
	[root@acyou hexo_blog]# git clone https://github.com/f981545521/hexo_blog.git
	[root@acyou hexo_blog]# cd hexo_blog/
	[root@acyou hexo_blog]# git pull
	[root@acyou hexo_blog]# npm install
	
	[root@acyou hexo_blog]# hexo generate
	[root@acyou hexo_blog]# hexo server
	-- 在后台运行
	[root@acyou hexo_blog]# nohup hexo server &
    // npx hexo <command>

   //链接至可执行文件：ln -s /root/apps/hexo_blog/node_modules/.bin/hexo /usr/local/bin/
   //运行：nohup hexo server -p 80 &
```
