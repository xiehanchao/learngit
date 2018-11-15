一、Git常用命令
01. git add 目录		   
    // 将目录下的文件添加到本地
02. git pull                                
    // 将master分支下的远程仓库中的git库文件最新版本pull下来，前提是没有修改当前目录下的git文件，若
03. git pull origin dev-conn    
    // 将origin dev-conn的分支下的代码pull下载下来
04. git pull --rebase                
    // 从暂存区把你之前提交的内容取出来，跟拉下来的代码合并，不会产生Merge的提交；
05. git commit -m “此次更新的概要”        
    // 为添加到本地的文件进行注释
06. git checkout -- WeChatAlbumApp/sensorBle/  
    // 将该目录下的文件还原成和git库中的一样
07. git log              
    // 检查git版本的log
08. git status         
    // 检查git版本的状态
09. git stash         
    //备份当前的工作区的内容，从最近的一次提交中读取相关内容，让工作区保证和上次提交的内容一致。同时，将当前的工作区内容保存到Git栈中。
10. git checkout -- 目录(DeviceManager/Zigbee)     
    // 将修改的部分还原到原来git库中的版本(修改部分不重要的情况下)
11. git diff              
    // 检查当前克隆的文件的修改的情况
12. git format-patch -s ed1ec367528f850f978        
    // 为当前已经提交到本地的git库文件打patch，可以不用将该文件上传到服务区，然后将该patch直接传给别人，放到相同的git库clone的目录下
13. git am 0001-sleepace-review.patch         
    // 将别人发过来的patch，放到相同的git库的目录下之后，执行该命令，即在代码中增加了patch，然后可以通过git log查看是否添加成功
14. git reset --hard dbb6e410b7123dcf315106f22e6a1ed3a3dc05c0        
    // 回滚到这个commit号的git代码文件状态下
15. git remote 不带参数，列出已经存在的远程分支
16. git remote -v | --verbose 列出详细信息，在每一个名字后面列出其远程url
17. git remote set-url origin <URL> 更换远程仓库地址。把<URL>更换为新的url地址。
    git remote set-url origin http://gitlab.frogshealth.com/albumapp-mini/albumapp-mini
15. git config --global user.name "ankie" 
    // 配置全局用户名，不加global就是本文件夹内的
	git config --global user.email ankie@health.com 
    // 配置全局用户邮箱
 	git commit --amend --reset-author 
    // 最后一次配置作者信息  	 
    git config user.name 
    // 查看当前用户名
	git config user.email 
    // 查看当前邮箱名
16. git fetch
    //刷新git服务器端的分支，更新本地的现有分支

