---
title: Hexo个人博客搭建笔记
date: 2017-03-31 16:40:03
category:
  - Hexo
  - init
tags: Hexo
---

## 运行环境搭建

### Node.js环境
Node.js开发者，早已配置好Node.js环境，本文不做重述。[前往学习](https://www.baidu.com)

### Git环境
工作、学习中依赖Git，环境搭建也不做重述。[前往学习](https://www.baidu.com)

<!--more-->

### Hexo环境
[官网文档](https://hexo.io/docs/)

下载安装Hexo客户端(生成管理工具)：
```bash
npm install hexo-cli -g
```

初始化一个Hexo项目：
```bash
hexo init hexo
```

进入项目所在目录：
```bash
cd hexo
```

安装npm依赖包：
```bash
npm install
```

安装可发布到git远程仓库的工具：
```bash
npm install hexo-deployer-git -S
```

初始化git项目(方便把源码上传到git)：
```bash
git init
```

关联远程仓库：
```bash
git remote add origin git@github.com:ImSiegeLion/ImSiegeLion.github.io.git
```

编辑 _config.yml 文件：
```yaml
deploy:
  type: git
  repository: git@github.com:ImSiegeLion/ImSiegeLion.github.io.git
  branch: master
```

预览效果：
```bash
hexo server
```
在本地浏览器地址栏中输入：localhost:4000

生成静态文件:
```bash
hexo generate
```

发布到git远程仓库:
```bash
hexo deploy
```