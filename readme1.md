##git
- 分布式

查看版本号
git --version

查看用户名和邮箱
git config --list

配置用户名和邮箱（告诉git 你是谁）
git config --global user.name 自己的用户名
git config --global user.email 自己的用户名

初始化git（想要哪个文件被git管理就在那个文件中初始化） 
git init 

创建目录
mkdir gitTest && cd gitTest(创建并进入)

查看文件列表
ls -l

查看所有文件列表和信息(包括隐藏文件)
ls -al

创建文件
touch index.txt

查看这个文件内容
cat index.txt

往文件中写入
vi index.txt
(默认不能编辑 按i键就可以编辑了 编辑完之后按esc键 在最下面按冒号+输入wq保存并推出)

查看git状态
git status

把文件加到暂存区内(.代表所有的)
git add .

提交到历史库
git commit -m

看git日志
git log
(不想看按q退出强制退出)

查看gi所有日志 
git reflog

对比代码
git diff（默认对比工作区和暂存区）
git diff --cached（对比暂存区和版本库）
git diff 分支名（对比工作区和版本库）

把文件从暂存区撤
git reset HEAD .

把文件从暂存区拉回工作区
git checkout 文件名

回到指定版本
git reset --hard 版本号（前7位就行）

查看所有分支
git branch

创建分支
git branch 分支名字

切分支
git checkout 分支名字

删除分支(前提是在其他分支)
git branch -D dev

创建并切换(相当于将当前内容克隆一份)
git checkout -b dev

合并分支(在主分支执行命令)
git merge dev 

产生冲突（手动解决，再提交）

清屏
clear

###创建仓库
- 创建空仓库，写一个仓库名字
new repository

本地要建一个readme.md   .gitignore
echo '.idea' >> .gitignore(把.idea追加到.gitignore)

搜索文件中带me的
git log --grep=me

查看
git remote -v

提交并关联仓库
git add .
git commit -m ''
git remote add origin 地址

删除
git remote rm o

查看所有关联
git remote -v

推送到远程仓库上
git push origin master -u（下次提交不用输origin master）






##svn
- 集中式