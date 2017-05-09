---
title: Hexo的部署
date: 2017-05-09 17：00
categories: hexo
tags: [hexo]
keywords: hexo
description: 学习hexo
---

# 1、安装必备软件 node.js git
# 2、安装hexo

```shell

npm install -g hexo
npm install hexo-deployer-git --save

hexo init

hexo clean (hexo c)

hexo generate (hexo g)

hexo deploy (hexo d)

```
# 3.配置_config.yml
```yml
deploy:
  type: git
  repository: https://github.com/tdyx87/tdyx87.github.io.git
  branch: master
```

# 4.支持图片
```bash
npm install hexo-asset-image --save
```
修改_config.yml

post_asset_folder: true
