# TestGit 

```bash
echo "# TestGit" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/heping945/TestGit.git
git push -u origin main
```

```bash
git branch develop master    # 从master分支上新建develop分支
git checkout develop    # 检出develop分支
# 此处可进行功能开发，并add和commit到develop分支
git push origin develop    # 推送develop分支到远端的origin/develop
```
