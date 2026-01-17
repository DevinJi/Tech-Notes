
# 本地配置多个git账户（公司与个人）
https://www.doubao.com/thread/w0e377165012506d7


1. 生成公钥/密钥对
ssh-keygen -t rsa -C "你的github绑定邮箱@xxx.com"
默认生成地方时~/.ssh/目录下面

生成式会提示
- 第1问：密钥保存路径和文件名 → 必须自定义，不要默认！
Enter file in which to save the key (/c/Users/xxx/.ssh/id_rsa): /c/Users/xxx/.ssh/id_rsa_gitlab
- 第2问：是否设置密钥密码（可选）→ 直接回车，空密码即可（免密登录）
Enter passphrase (empty for no passphrase): 
- 第3问：确认密码 → 直接回车
Enter same passphrase again: 

2. 编辑config文件.  如果配置多个git账号，则在这里面配置 Mac/Linux

vim ~/.ssh/config
```
Host github.com
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa_github  # 对应个人GitHub的私钥文件名
```

3. 测试联通性：
ssh -T git@github.com
