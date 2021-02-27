### [user]
        email = keke@qq.com
        name = keyongteacher  

### [alias]
        ci = commit
        st = status
        ad = add .
        hi = log --pretty=format:'%h %ad | %s%d' --graph --date=short

### git config --list
    git config --list
    git config --gloabl alias.ci=commit
    git config --global credential.helper wincred  可以保存https协议每次输入密码的麻烦

### ssh协议生成密钥命令
    ssh-keygen -t rsa -C "3375630896@qq.com"

    把公钥放到github网站上
    cat ~/.ssh/id_rsa.pub

    profile-setting-ssh and gpg keys

### 列出常用命令
    git

    列出所有子命令
    git help -a

    列出文件修改历史记录
    git blame filename
    git blame -L 0,100 filename

### 列出要清除的文件
    git clean -n 
    清除文件
    git clean -f
    git clean -x
    会清理gitignore的内容

    git status -sb short branch 简短的列出变更

    git rm 删除文件
    git mv 重命名或移动文件
    git reset hash | head 撤回到某个commit  

### git show HEAD 显示当前提交的变更 
    git show HEAD^ 上一个提交  HEAD^^上2个提交，也可以写为HEAD~2
    git diff 

### git commit 规范
    type(scope):fix xxx 

    body 

    footer 

    示例
    docs(file):fix file

    close #1  关闭bug  

    git hi filename (git config --global alias.hi=log 这个命令) 可以看到这个文件的提交历史记录

### git diff  
![diff](./log/diff.png)



### HEAD 代表当前的commit
    HEAD^ 代表上一个commit
    HEAD^^ 代表上2个commit = HEAD~2

    git show HEAD
    git hi fileme
    git blame filename
    git diff HEAD  workingdirector commit  当前工作区和最新commit的区别
    git diff --cache  index/stage  commit  当前暂存区和最新commit
    git diff workdirectory index/stage     当前工作区和暂存区
    git diff HEAD^ HEAD^^ commit1 commit2  当前commit1,commit2的区别
### git tag 
    git tag tagName commit 在某个提交上面打标记
    
    在某个提交上面commit
    可以
    git show
    git diff
    git tag  




