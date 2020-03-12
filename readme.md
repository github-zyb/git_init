<!-- 这是第1个功能，基本命令 -->
git init	//初始化仓储
git config --global user.name "zyb"	  //配置姓名
git config --global user.email "919541244@qq.com"   //配置邮箱
git add ./readme.md 	//将需要备份的文件放到仓储大门口
git commit -m "这是一些说明！！！"	//将文件放到仓库的一个房间

<!-- 这是第2个功能，附加的重要命令 -->
git status	  //查看状态
git add ./	  //将所有修改的文件全部添加到暂存区
git commit --all -m "这是一些说明！！！"	//将暂存区的文件放入版本库，跳过暂存区的命令
git log		//查看提交日志
git log --onelinbe		//将日志信息捡关键的在一行中显示，方便查看

<!-- git通过head指向回退恢复指令 -->
git reset --hard Head~0		//恢复到版本0



<!-- git通过版本号恢复 -->
git reset --hard "版本号"

<!-- 输出操作的所有Log,查询版本号 -->
git reflog



<!-- 子分区操作 -->
git branch "分支名"		//创建分支
git branch 				//查看分支
git checkout "分支名"	//切换到某分支
任务完成后
git checkout master		//回到主分支
git merge dev			//将子分支dev与主分支进行合并


<!-- 冲突处理 -->
git branch -d "分支名"

<!-- 提交代码到github（当做git服务器来用） -->
git push [地址] master

<!-- 使用pull下载代码文件 -->
git pull "地址"(https://github.com/github-zyb/git_init.git) master

<!-- 使用clone下载代码文件 -->
git clone "地址"（https://github.com/github-zyb/git_init.git） 


<!-- 配置远程，目的是为了简化操作 -->
git add remot [自拟变量名] （https://github.com/github-zyb/git_init.git）		//配置命令
git push -u master		//配置完之后，使用此命令即可上传
git push		//下一次执行这个命令就相当于执行上面一行的命令
git pull		//在同一个工程目录下下载只需使用这行代码即可
必须在同一个目录下	