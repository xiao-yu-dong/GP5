# readme文档
- 项目说明文档
- 一般都与项目放在一起

# git操作

## 初始化版本库
- git init
- 初始化成功后，当前目录后面有（master）
- 初始化成功后当前目录下有一个隐藏文件.git（不要管，不要操作这个文件）

## 工作区（所看到的文件，代码就是工作区）
- 持有实际文件
- 我们平时增删改查的文件都是工作区的内容

## 暂存区
- 可以理解为我们看不到的地方
- 本地仓库的一个主要组成部分

## 本地仓库
- 可以理解为我们看到的一个地方
- 也是存在于用户电脑中的
- 用户存储项目代码及版本项目记录信息

## 提交到暂存区
- git add . 文件名
- 用于将工作区的变动提交到暂存区
- git.dd 将所有变动提交到暂存区

## 查看状态
- git status
- 查看工作区和暂存区的状态（增删改）

## 提交到本地仓库
- git commit -m '提交注释'
- 将代码从暂存区提交到本地仓库

## 查看配置列表
- git config --list
- git status 查看状态提示：工作区是干净的，没有任何东西需要提交（表示完成）
- 

## 本地操作关键步骤
1. git init  初始化之后，不需要再初始化（第一次需要）
2. git add .
3. git commit -m '注释' 