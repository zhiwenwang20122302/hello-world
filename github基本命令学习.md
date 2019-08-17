# github基本命令学习

> Author : Zhiwen Wang   
> Email: zwwang@my.swjtu.edu.cn  
> Tell: 15708418408  
> QQ: 1042261073  
> WeChat: wzw_20122302  
>Address: Chengdu China 611756  
> [Home Page ](http://192.168.9.5/zhiwen.wang) `http://192.168.9.5/zhiwen.wang`  
> [Github](https://github.com/zhiwenwang20122302)

## 生成秘钥 
> [参考网址](https://help.github.com/en/articles/connecting-to-github-with-ssh)  
> 在本地服务器上 运行  
> 这里需要自己准备一个密码 

## 复制写到网页上
> ssh

## git初始化
* git config --global user.name "zhiwenwang20123202"
* git config --global user.email "zhiwenwang20122302@gmail.com"
* git clone git@github.com:zhiwenwang20122302/hello-world.git
* 这里需要输入密码，和自己上面设置的密码保持一致

		
## 本地文件编辑后同步到远程github
### 编辑
* vi READM.md
*  add "this is third time to update my file"
### 更新
* git add .
* git commit -m 'update'
* git push -u origin master
* 输入密码

## 远程github文件编辑后同步到本地
### 编辑
* 网页上可是化编辑
### 同步到本地
* git pull
* 输入密码


192.168.9.19:/DATACENTER1/zhiwen.wang/githubtest/hello-world 和远程服务器文件同步

192.168.9.5:/DATACENTER2/huifu-project 和实验室gitlab同步
