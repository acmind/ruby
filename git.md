## 配置Git

    $ git config --global user.name "Your Name Here"
    # 设置默认用户名

    $ git config --global user.email "your_email@example.com"
    # 设置默认邮箱

    $ git config user.name 
    $ git config user.email
    # 在上述设置完毕后，可通过这两条命令查看自己的设置

## 创建仓库

    # 远程：
        
        首先在 Github.com 上创建一个repository （例：Hello-World）

    # 本地：
    
        $ mkdir ~/Hello-World
        # 在本地的~/目录下创建一个 git 仓库，目录创建在别处也可以

        $ cd ~/Hello-World
        # 切换至刚创建好的目录

        $ git init
        # 初始化一个本地的 git仓库，生成隐藏的.git目录

        # 添加：

            $ touch README
            # 可以添加.txt .md .html等格式后缀,找到后可打开编辑。

            $ git add README
            # 把README文件添加到仓库中

            $ git commit -m 'first commit'
            # 执行提交说明

        # 提交：

            $ git remote add origin https://github.com/username/Hello-World.git
            # 使用https协议指定、连接远程仓库地址

            $ git push origin master
            # 推送本地仓库到远程指定的master主分支上