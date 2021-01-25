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
- 可以理解为我们看不到的一个地方
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


## 查看操作日志
- git log    完整版日志
- git reflog 简单版日志

## 版本回退
- git reset --hard HEAD^  （回退上一个版本）
- git reset --hard 版本号  ‘1c030a8’  （回退到指定版本）
- 工作区自动变为指定版本的代码
- 注意把当前代码先提交到本地仓库

## 查看变动信息
- git diff '文件名'
- 会列出该文件前后的差异

## 创建远程仓库
- 进入 github官网
- 创建一个新的远程仓库

## 将本地仓库与远程仓库关联
- git remote add origin https://github.com/xiao-yu-dong/GP5.git 你的远程仓库地址  （设置，关联地址）
- git remote -v  查看本地仓库关联的远程仓库地址

## 将本地仓库提交到远程仓库
- git push -u origin master 第一次提交到远程
- git push 将本地仓库提交到远程仓库
- -u origin master 设置默认的提交地址和分支

## 清屏
- git clear

## 正常提交（非第一次）
- git add . 提交到暂存区
- git commit -m '注释' 提交到本地仓库
- git pull 先更新远程到本地
- git push 提交到远程仓库（默认提交到origin上的master分支）

## 修改关联的远程仓库地址
- git remote rm origin    删除远程地址
- git remote add origin ssh地址      添加新的地址

## 更新代码
- 确保自己工作区的代码先提交到本地仓库
- 然后再从远程更新到本地  git pull 
- git clone 远程仓库地址 （克隆代码到本地）


## 分支
- git branch  查看当前所有分支
- 当前分支名前有一个星号
- git branch ‘分支名’  创建一个分支
- git checkout ‘分支名’  切换分支
 