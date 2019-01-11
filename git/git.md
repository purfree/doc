### 查看远程仓库地址
git remote -v
### windows git clone输入错误密码被保存后，如何修改
打开控制面板->用户账户->凭据管理器，windows凭据。  
根据git地址找到对应的内容，修改或删除密码。
### git clone 账号和密码
git clone http://username:password@url
### 回滚到指定版本,不保留历史记录
git reset --hard 版本号  
git push origin master -f
### 修改全局配置
git config --global user.name "yourname"  
git config --global user.email "youremail"
### 修改本地配置
git config user.name "yourname"  
git config user.email "youremail"
### windows 给文件添加执行权限
git update-index --chmod=+x exe
### 本地分支重命名
> git branch -m oldName newName
### 远程分支重命名
1. 本地分支重命名
> git branch -m oldName newName
2. 删除远程分支
> git push --delete origin oldNam
3. 上传新命名的本地分支
> git push origin newName
4. 把修改后的本地分支与远程分支关联
> git branch --set-upstream-to origin/newName 