
# git使用指南


一、创建版本库
```
git init 创建版本库
```
git add  将文件添加到仓库
```
git commit -m  "此处填写描述"  将文件提交到仓库
```

二、版本回退
```
git  log   查看历史提交记录
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

