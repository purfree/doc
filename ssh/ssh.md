## 将密钥添加的高速缓存中，避免每次输入密码。
eval $(ssh-agent -s)   
ssh-add ~/.ssh/id_rsa
