# Git 教程

此教程用来记录学习，内容来自B站 **cjxz-2019 **

https://space.bilibili.com/405560716?spm_id_from=333.788.b_765f7570696e666f.2

用来记录学习

## 1.git环境搭建

### 1.1.安装git软件

●下载git安装文件 [ https://git-scm. com/ download/ mac]( https://git-scm. com/ download/ mac)   或者去镜像下
[镜像](https://www. newbe . pro/Mirrors/Mirrors-Git-For -Macos/) 
●测试git是否安装成功 git --version !

```c++
zhuchaodeMacBook- -Pro-2:- zhuchao$ git --version
git version 2.17.2 (Apple Git-113)
```

### 1.2.配置基本信息

```c++
git config --global user.name '你的用户名'
git config --global user.email'你的用户邮箱'
```

作用:配置好这些信息后当你提交文件的时候就有提交人，这里的提交人就是取得config的配置文件。除了 使用--global外git还提供了两种设置，但是不常用分别为:

​			`●-ocal: 只对某个仓库生效`

​			`●--system: 对系统所有登录用户有效`

​			`●-global: 对当前用户的所有仓库有效`

### 1.3.查看配置基本信息

```c++
git config --list
git config --list --g1obal
git config --1ist --1ocal
git config --list --system
```

### 1.4.建git仓库



### 1.5.修改已经配置的全局信息



***

## 2.git常用命令

### 2.1.git 工作目录

​	工作区	-->	暂存区	-->	历史版本 

### 2.2.提交文件常用命令

```c++
//将文件从工作区提交到暂存区
git add 文件名
//将所有变更工作区提交到暂存区
git add -A 
git add *
//提交暂存区内容
git commit -m '单引号里面是注释，用来解释此次提交'
//查看工作目录状态
git status
//重命名文件
git mv 源文件 新文件名称 
//创建分支
git branch 新分支 源分支
//查看分支
git branch -av
//切换分支
```

### 2.3.git日志

```c++
//查看当前分支的历史
git 1og
//查看当前分支简介的历史
git log --oneline
//查看最近两次历史记录
git log -n2
//查看当前有多少个分支
git branch -v
//查看所有分支所有历史
git log --all
//带图形界面的方式查看git
git log --graph
```

## 3.git如何管理文件

### 3.1.查看.git文件夹

#### 3.1.1.HEAD

#### 3.1.2.refs

#### 3.1.3.config

#### 3.1.4.object文件夹

### 3.2.git对象

### 3.3.git中commit/tree/blob关系

### 3.4.三者关系

### 3.5.深入认识HEAD和branch

#### 3.5.1.案例分离头指针

#### 3.5.2.HEAD的作用

#### 3.5.3.比较暂存区和HEAD的区别

#### 3.5.5.比较两个分支的差异

#### 3.5.5.删除分支

### 3.6.使用rebase修改提交记录

3.6.1.修改历史提交记录的message信息

3.6.2.合并几次提交记录

### 场景？？？

### 3.7.回滚

#### 3.7.1.恢复暂存区跟HEAD保持一致

#### 3.7.2.恢复工作区跟暂存区保持-致

#### 3.7.3.部分恢复暂存区文件跟HEAD保持一-致

#### 3.7.4.回滚commit

#### 3.7.5.试炼项目中回滚场景

### 3.8.删除文件

### 3.9.临时加塞任务怎么处理

### 3.10.忽略文件

#### 3.10.1.如何使用.gitignore文件

#### 3.10.2.查看github.上面常用的忽略文件

### 3.11.备份

#### 3.11.1常用的备份方式

#### 3.11.2试炼备份

## 4.github

### 4.1.github环境设置

#### 4.1.1.注册账号

#### 4.1.2.设置ssh

### 4.2.本地代码同步到远程仓库

### 4.3.将远程仓库代码拉到本地