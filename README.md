
## 本地 连接 github 初始化一个项目
```bash
echo "# TestGit" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main         # 将默认分支 从 main改为 main
git remote add origin https://github.com/heping945/TestGit.git      # 关联
git push -u origin main                 # 以后 可以 直接 git pull 或者 git push
```
## 创建 切换 查看 分支 
```bash
git branch dev main    # 从main分支上新建dev分支
git checkout dev    # 切换到dev分支
## git branch 查看当前所处 分支 带* 的是当前分支
git push origin dev    # 推送develop分支到远端的origin/develop
```
## 线上代码热更新，开一个 分支，修改，merge ，适合一些小的bug
```bash
git checkout main    # 切换回main分支
git checkout -b hotfix main    # 新建hotfix分支，并切换到该分支
......                 # 做一些bug修复工作
git checkout main    # 切换回main分支
git merge --no-ff hotfix    # 合并hotfix分支，此时bug已被修复（无冲突）
git tag v0.2    # 新建tag v0.2
git add . && git commit 
git push origin main    # 推送main分支代码到远端
git push origin --tags    # 推送tag到远端
```

