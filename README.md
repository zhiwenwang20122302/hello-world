# how to used git for leaning
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


# hello-world
 
welcome to my github page!

Let's start with deep learning!

this is my second time to update my file!

thie is my third time to update my file!

this is my fourth time to update my file! 

i am in microsoft!!!
