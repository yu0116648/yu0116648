# GitHub学习笔记

## 仓库

* 仓库是存放代码的文件夹，分为公开仓库和私有仓库两种： 
  * 公开仓库（Public）：所有人可见，比较适合开源项目。
  * 私有仓库（Private）：指定人员可见，适合个人，企业，团队项目，可能会需要付费

## 分支

* 分支是项目的并行开发线，默认主分支是main，主要用于开发新功能，修复bug，避免直接修改主分支代码

## 提交

提交是代码的快照，每次修改后通过commit保存，并且修改后填写修改描述信息，以便于快速追溯历史

## 请求

Pull Request，简称PR，是将分支代码合并到主分支的申请，可以对代码进行审查，讨论，确定代码质量

## 克隆

将远程仓库上的代码复制到本地的电脑，便于进行本地开发

## 本地仓库操作

* 初始化本地仓库 git init  在当前文件夹创建git仓库

* 查看文件状态 git status 显示文件的修改、暂存、跟踪状态

* 暂存文件  git add 文件名 暂存当前文件夹所有修改的文件

* 提交暂存文件 git commit -m”提交描述“保存暂存的修改

* 查看提交历史get log or get log --oneline 以简洁格式显示历史

   

## 远程仓库操作

* 克隆远程仓库到本地 git clone 远程仓库URL
* 关联本地仓库到远程 git remote add origin 远程仓库URL 首次将本地仓库推到GitHub时使用
* 查看远程仓库关联 git remote-v 显示已关联的远程仓库URL
* 拉取远程仓库代码 git pull origin分支名 同步远程分支到本地
* 推送本地代码到远程 git push origin 分支名
* 查看远程分支 git branch-r 显示远程仓库的所有分支
* 切换到远程分支 git checkout-b 拉取远程分支并在本地创建对应分支



## 分支操作

* 查看本地分支  git branch
* 创建并切换分支 git checkout-b 新建分支并切换到该分支
* 切换已有分支 git checkout分支名
* 合并分支到当前分支 git merge 待合并分支名
* 删除本地分支 git branch-d 分支名
* 删除远程分支 git push origin --delete 远程分支名 删除GitHub上指定分支



