
------
# git是什么
是一个分布式版本控制系统（svn为集中式）
{% post_link hexo-tutorial  hexo教程%}
[hexo](hexo-tutorial.md) 
------
# github是什么
- 一个网站
- 提供git仓库服务
- 有很多程序员乃至公司在github分享代码
- 全球最大的同性交友平台^-^

------
# 安装
非常简单。前往[git官网](https://git-scm.com/)找到适合自己平台的软件，进行安装。


------
# 重要概念

- ssh、公钥、私钥
- 暂存区
- 本地仓库
- 远程仓库
- 主干、分支、合并
- 冲突、解决冲突


------
# 常用命令

### 显示帮助
```
git config --help # 这里以config指令为例，查看config指令的使用帮助 
```

### 初始化git仓库
```
git init
```

### 查看状态
```
git status 
```

### 添加至暂存区
```
git add filename  # 指定单个文件。将这个文件变动添加至暂存区

git add *.js  # 使用通配符指定多个文件。将.js结尾的文件变动添加至暂存区

git add -A  # 将所有变动添加至暂存区
```

### 提交
```
git commit -m 'describe something about this commit'
```

### 查看差别
```
git diff
```

### 查看log
```
git log # 查看log
git log --graph #以图形的形式查看log
git reflog 
``` 

### 创建分支并切换过去
```
git checkout -b branchName
```

### 合并分支
```
git merge branch-a # 将branch-a分支合并到主分支 
```

### 克隆一个仓库
```
git clone # 这里以github上的仓库为例
```

### 从远程仓库获取最新代码
```
git pull
```

### 提交本地代码到远程仓库
```
git push
```

### 关联远程仓库
```
git 。。。。
```


------
# 参考资料
- [git官网推荐的资料](https://git-scm.com/doc)
- [github入门与实践](https://book.douban.com/subject/26462816/)