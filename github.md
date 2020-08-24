# 如何使用git和github.com
***********************
1. 什么是git/github
    - git:版本控制工具，为代码记录一个个版本
    - github：代码托管平台，类似于网盘

2. git的安装和github的注册
    1. 下载git的安装包，根据提示安装
    2. 在github.com注册账号（sign up）记住**用户名、邮箱和密码**    
    3. 打开git bash终端，配置git
        - git config --global user.name "your registered name"
        - git config --global user.email "your registered eamil"

3. 在github上创建项目，得到项目的地址
    - 登录(sign in)github.com 点击右上角+ New Repository 填写项目名称和描述
    - 捕获github项目的地址 https://****.git
    - 在**本地**待上传的文件夹右键，打开git bash终端 （即cd destinational folder）

    - 依次输入以下命令（第一次）
        1. git init  # 初始化该项目的版本控制，生成.git隐藏的文件夹
        2. git add . # 将当前目录下的所有文件（夹）提交的暂存区
        3. git commit -m "提交该版本的描述信息"
        4. git remote add origin https://****.git  # 本地git和github建立联系
        5. git push -u origin master # 根据提示在本地登录github，随后自动进行网络传输
        
4. 使用git记录多个版本
    - 在git bash中重复执行add,commit,push指令即可
        1. git add .
        2. git commit -m "第n个版本的说明信息"
        3. git push origin master
    
