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
$ git reset 
```

## 强制重制方法

用于同步原作者的commitId。

```bash
$ git reset --hard commitid
$ git push -f master
```

## rebase用法

用于合并自己本地分支的冗余commit，指定一个为最终commit。

```bash
$ git rebase -i commitid
```

或者合并最新的两个分支。

```bash
$ git rebase -i HEAD~2 
```

## 各大著名贡献指南

- [Vuejs贡献指南中文版](./.github/CONTRIBUTING.md)
- [Angular.js贡献指南](https://github.com/angular/angular.js/blob/master/CONTRIBUTING.md)
- [Reactjs贡献指南](https://reactjs.org/docs/how-to-contribute.html)
- [Webpack贡献指南](https://medium.com/webpack/contributors-guide/home)
