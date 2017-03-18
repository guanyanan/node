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
(不想看按q退出)

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


清屏
clear

##svn
- 集中式