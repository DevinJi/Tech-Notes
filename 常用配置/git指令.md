# 笔记常用指令

1. 第一步：git add .  → 把本地所有新增/修改的笔记文件，加入「暂存区」
git add .

2. 第二步：git commit -m "备注信息" → 提交到本地仓库，备注写清楚本次做了什么 ✅ 备注规范：简洁明了，比如 新增Python路径笔记、修改Git密钥配置、补充dashscope代码
3. git commit -m "新增Python file路径写法笔记 + dashscope多模态基础用法"
 第三步：git pull → 先拉取云端最新版本（防止多人协作冲突，自己记笔记也建议加，好习惯）
```git pull```

4. 第四步：git push → 把本地笔记推送到GitHub云端，完成同步！
```git push```


![alt text](image.png)
# 配置当前工程名称 提交代码的名称
  Tech-Notes git:(main) ✗ git config --local user.name DevinJi
➜  Tech-Notes git:(main) ✗ git config --local user.email 365157975@qq.com