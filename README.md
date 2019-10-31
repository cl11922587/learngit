
# git使用指南


一、创建版本库
```
git init 创建版本库
```
git add  <文件活目录明>  将文件添加到仓库
```
git commit -m  "<此处填写描述>"  将文件提交到仓库
```

二、版本回退
```
git  log   --pretty=oneline --abbrev-commit 查看历史提交记录
```
git reset --hard HEAD^  OR git reset --hard HEA~100  回退到上个版本或者 前100个版本
```
git reflog  找到所有历史记录
```
git status  查看状态
```
git diff  对比工作区与版本库区别
```
git checkout  撤销修改，把文件恢复到上个版本状态
```
```
git rm  <文件或者目录> 删除无文档
```


三、远程仓库
```
git remote add origin  <仓库地址>  关联远程仓库
```
git push -u  <远程仓库默认：origin> <本地分支：master>  推动远程仓库。第一次需要 -u
```
git clone <仓库地址>  克隆远程仓库
```
$ git remote -v查看远程仓库信息
```

git pull  拉取远程最新的提交
```
四、分支管理
```
git branch <分支名称|空>   创建分支|查看所有分支
```
git checkout|switch <分支名称>    切换分支
```
git checkout|switch  -b <分支名称>    创建+切换分支
```
git merge <分支名>   将分支合并到当前所在分支上
```
git branch -d <分支名称> 删除分支
```
git merge --no-ff -m "merge with no-ff" <分支名>   强制禁用Fast forward模式
```
git stash <空>|list|apply|drop|pop   存储当前工作现场|查看工作现场|恢复工作现场|删除现场|恢复加删除，等恢复后继续工作， 常用语紧急BUG修复
```
git cherry-pick <分支提交信息>  将分支提交的内容合并到当前分支
```
git tag 用于创建一个标签，
```
