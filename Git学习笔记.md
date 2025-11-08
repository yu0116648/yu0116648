# Git学习笔记

## 基础配置

* 配置用户信息

1. git config --global user.name "你的用户名"

2. git config --global user.email "你的邮箱"

* 查看配置信息
  * git config --list   查看所有配置

## 核心工作流程

* Git 工作区分为工作区（本地文件）、暂存区（index）、本地仓库（.git）、远程仓库（GitHub）
* 核心流程：修改文件>暂存>提交>推送

##  常用核心命令

1. 仓库操作
   * 初始化本地仓库：git init 新建文件夹，生成.git目录
   * 克隆远程仓库：git clone<远程仓库地址>
   * 关联远程仓库：git remote add origin<远程仓库地址>
   * 查看远程仓库：git remote-v

2. 暂存与提交
   * 查看文件状态：git status
   * 暂存文件;git add<文件名>
   * 取消暂存：git reset HEAD<文件名>
   * 提交到本地仓库：git commit-m 说明需清晰
   * 查看提交记录：git log
3. 分支操作
   * 查看分支：git branch
   * 创建分支：git branch<分支名>
   * 合并分支：git merge<待合并的分支名>
   * 删除分支：git branch-d<分支名>
4. 远程同步
   * 拉取远程代码：git pull origin<分支名>
   * 推送本地代码：git push origin<分支名>
   * 查看远程分支：git branch-r



## 使用Git Bash提交并推送到远程仓库

1. 在git上配置用户名和邮箱
2. 选中要上传的文档（需要保存在文件夹中，直接选中文件夹），右键点击文件夹，显示更多选择git bash
3. 命令行中输入 git init，并回车
4. 命令行中输入 git add .，并回车
5. 命令行中输入git commit-m"任意字符"将文件提交本地仓库，并回车
6. 命令行中输入git remote add origin 仓库地址，并回车
7. 命令行中输入 git pull origin main（有些为master，根据实际情况选择），并回车
8. 命令行中输入git pull origin main（有些为master，根据实际情况选择） --allow-unrelated-histories（若READE文件已存在）并回车
9. 命令行中输入 git push -u origin main（有些为master，根据实际情况选择）进行推送
10. 打开提交到的GitHub远程仓库，刷新后

## 其他提交方式

GitHub提交方式比较麻烦，对于初学者而言，对git的命令掌握的不是很熟悉，不会使用，甚至都找不到命令行入口，即使找到了入口在输入的时候也会遇到各种各样的报错，如果没有足够的经验和强大的外部工具的支持和自己的出色的理解能力，很难在短时间完成文件的提交。



通过查阅资料，我了解到还有以下几种提交方式：

* VS code内置的git功能，在左侧源代码管理面板，可以直接暂存、填写提交描述、推送、并且能实时显示文件修改差异
* Git GUI:右键本地仓库，选择Git GUI Here，可以较为直观地完成暂存、提交、推送和分支的切换
* Sourcetree：可以进行分支管理、PR查看、冲突解决，适合团队协作。

