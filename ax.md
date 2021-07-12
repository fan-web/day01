## 作业

* 1、注册Github账号，并把注册邮箱发给同时@老师。

* 2、下载安装Visual Studio Code编辑器 https://code.visualstudio.com/ 。

## 场景一：把现有的项目或新项目用Git管理

```
$ mkdir test
$ cd test
$ git init
$ touch index.html
$ git status
$ git log
$ git add index.html
$ git status
$ git commit -m "add index.html"
$ git log
$ git remote add origin 你自己的远程仓库url
$ git push -u origin master  (第一次提交的时候才需要加-u origin master，以后可省略，直接git push)
```

## 场景二：从远程仓库克隆到本地（推荐！！！）

```
$ git clone 远程仓库url
$ cd 仓库目录
$ touch README.md
$ git status
$ git log
$ git add README.md
$ git commit -m "add README.md file"
$ git push
```
