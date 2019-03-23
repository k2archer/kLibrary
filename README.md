# 图书管理系统

[TOC]



#### 项目描述

**What is kLibrary?**

一个图书管理系统，实现一个基本的 C/S 架构系统。
C++ 实现简单静态 Web 服务器，MySQL 作为后端数据库，通过 CGI 接口，使用 Python 实现动态脚本支持。
在 Android 端实现客户端，通过 HTTP API 连接服务端进行通信交互。

实现基本功能模块：登录、~~注册~~、已订阅列表、~~推荐列表、搜索书籍、收藏列表、系统消息、个人中心~~。

[详细设计开发文档](docs/index.md)

**Features**

* C/S 架构
* 支持 Android ~~和 Web~~ 客户端

#### 编译&运行

**Required**

*  MySQL

**Building**
* clone projects
```
git clone https://github.com/k2archer/kLibrary.git
git submodule foreach git pull
```

* submodule project

```
#server https://github.com/k2archer/kWeb
#client https://github.com/k2archer/iLibrary
```

