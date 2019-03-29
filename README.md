# Contributing Guide

## 第一步：fork原作者的项目

略

## 第二步：clone自己fork之后的版本

```bash
$ git clone -o yourself https://github.com/yourself/project.git
```

参数说明:

```
-o <name>

Instead of using the remote name origin to keep track of the upstream repository, use <name>.
```

## 第三步：将原作者的仓库远程地址添加到本地

```bash
$ git remote add author https://github.com/author/project.git
```

查看有哪些远程仓库：

```bash
$ git remote -v
```

## 第四步：同步原作者的仓库改动

```bash
$ git pull author master
```

## 强制重制方法

慎用

```bash
$ git reset --hard commitid
$ git push -f master
```

## rebase用法

## Vue.js 贡献指南中文版

[移步](./.github/CONTRIBUTING.md)
