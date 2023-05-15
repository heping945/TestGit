# TestGit 

```bash
echo "# TestGit" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main         # 将默认分支 从 master改为 main
git remote add origin https://github.com/heping945/TestGit.git      # 关联
git push -u origin main                 # 以后 可以 直接 git pull 或者 git push
```

```bash
git branch dev main    # 从main分支上新建dev分支
git checkout dev    # 切换到dev分支
## git branch 查看当前所处 分支 带* 的是当前分支
git push origin dev    # 推送develop分支到远端的origin/develop
```
