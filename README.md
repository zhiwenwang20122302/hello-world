# 如何使用github配合ubuntu服务器开发
    [学习文档，来自北京航天航空大学的Si Liu老师的总结](https://github.com/siliu-group/document)

## 配置github
### 方式1 本地记住密码
 
    # 用户名
    git config --global user.name "zhiwenwang20122302"
    # 邮箱
    git config --global user.email "zhiwenwang20122302@gamil.com"
    # 设置记住密码
    git config --global credential.helper store

### 方式2 ssh登录记住密码

    # 这种方式需要利用一堆秘钥对进行认证
    # 生成秘钥对，一路回车
    ssh-keygen -t rsa
    # 查看公钥
    vim  ~/.ssh/id_rsa.pub 或 vi ~/.ssh/id_rsa.pub
    # 复制终端显示的公钥，然后:q!退出
    # 将复制的公钥添加到github setting->SSH and GPG key->New SSH key

## 新建git仓库

    # 第一种 现在本来init了一个仓库然后和远程仓库进行连接并拉取文件下来
    mkdir dirname
    git init
    # git remote add <主机名> <网址>
    git remote add origin https://github.com/zhiwenwang20122302/hello-world.git
    # git pull <远程主机名> <远程分支名>:<本地分支名> 尽量保持远程分支名和本地分支名一致
    git pull origin master:master
    # 第二种 直接clone
    git clone https://github.com/zhiwenwang20122302/hello-world.git

## 更改文件并提交

    # 比如你新加了一个readme.txt文件
    # 首先把你要提交的改动add到暂存区
    git add readme.txt
    # 可以同时add多个文件
    git add readme.txt readme2.txt
    # 将当前目录说有文件add进暂存区
    git add .
    # 然后将暂存区的文件提交到本地仓库
    git commit -m “本地提交的log”
    # 将本地仓库的改动push到远程仓库
    # git push <远程主机名> <本地分支名>:<远程分支名>
    git push origin master:master

## 更多内容参考si liu的文档
