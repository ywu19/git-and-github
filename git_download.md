[toc]
##  1. 目的
手机用git管理GitHub托管项目代码
## 2. 下载安装
git官网：https://git-scm.com/download/win
检验：桌面鼠标右击出现两个git则安装成功
## 3. 工作流程
### * 工作区域
* 工作区（Working Directory）：添加、编辑、修改文件等动作
* 暂存区：暂存已经修改的文件，最后统一提交到git仓库中
* Git仓库（Git Repository）：最终确定的文件保存到仓库，成为一个新的版本，并对其他人可见
### * 工作流程

## 4. Git初始化、仓库创建与操作
### 1. 基本信息设置(git config --global)
#### 1-1 设置用户名
> git config --global  user.name 'ywu19'  
git config --global参数对此电脑上所有git仓库都是用此配置 
#### 1-2 设置用户邮箱
> git config --global  user.email '3140575572@qq.com'

#### 1-3 查看设置（是否初始化）
> git config --list

### 2. 初始化一个新的Git仓库
#### 2-1 创建文件夹
> 桌面新建文件夹--右键Git Bash--mkdir test 
#### 2-2 在文件夹内初始化git (git init)一次即可
> cd test
git init  
test文件夹内显示隐藏文件.git

### 3. 向仓库添加文件
#### 3-1 创建文件
>  touch a2.md
git status  


#### 3-2 添加到暂住区 (git add)
> git add a2.md
git status  


#### 3-3 将文件从暂住区提交到仓库 (git commit -m ' ')
> git commit -m 'add a2.md'
git status  


### 4. 修改仓库文件
#### 4-1 修改文件
> vi a2.md
git status  


#### 4-2 将修改文件添加到暂住区
#### 4-3 将修改文件从暂住区添加到工作区


### 5. 删除创建文件
#### 5-1 删除文件
> rm -rf a2.md  
#### 5-2 从git中删除文件
> git rm a2.md  
#### 5-3 提交操作
> git commit -m '提交描述'

## 5. Git 管理远程仓库
使用远程仓库的目的：备份，实现代码共享集中化管理



#### Step1  Git 克隆操作( git clone)   
目的：将远程仓库（GitHub对应的项目）复制到本地
代码
> git clone 仓库地址
仓库地址由来


或者通过ssh
>  ssh-keygen -t rsa -b 4096 -C "3140575572@qq.com"
clip < ~/.ssh/id_rsa.pub  



#### Step2 本地仓库内操作
#### Step3 同步到git远程仓库中(git push)
> git push  

## 6.Github Pages 搭建网站
### 1 个人站点
#### 1-1 访问
> https://用户名.github.io
https://ywu19.github.io      
#### 1-2 搭建步骤
1. 创建个人站点 --->新建仓库（仓库名必须是【用户名.github.io】）

2. 在仓库下新建index.html的文件即可
注意此仓库里只能是HTML文件
### 2 项目站点
#### 2-1 访问
> https://用户名.github.io/仓库名  
#### 2-2 搭建步骤
1. 进入项目主页--> 点击settings
2. 在setting页面，点击








