### 安装芒果云 到目录 e
wget "https://github.com/kalcaddle/KODExplorer/archive/master.zip"

### c9的sshkey 加入 github 的项目的 deploy key 中

### git 初始化

git init
git config --global user.name "Your Name Here"
git config --global user.email "your_email@example.com"
git remote add origin git@github.com:ansediao/wptest.git
git fetch origin  master
git merge origin/master --allow-unrelated-histories


### git 推送 
git add .
git commit -m 'init' 
git push


### release 
> 先打标签
> 后推送这个标签

git tag -a v0.1.2 -m "v0.1.2版本"
git push origin v0.1.2