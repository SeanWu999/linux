# linux命令

(1) sudo chmod -R 777 wuzhe/  解锁wuzhe下的权限，777是最大的       chmod u+x filename 使文件有可执行权限

(2) python3 编译pyc python3 -m compileall -b .

(3) python2 编译pyc python -m compileall .

(4) lib****.so.10报错，用以下语句重置  sudo ldconfig /usr/local/cuda-10.0/lib64 （在使用编译后的caffe，openpose时出现的）

(5) grep Aug /var/log/messages 在文件 '/var/log/messages'中查找关键词"Aug" 

(6) ubuntu18 配置静态IP： '参考1' [website](https://blog.csdn.net/qq_34889607/article/details/82497405)，'参考2' [website](https://www.jianshu.com/p/2b401aa0052d)

(7) ubuntu16 安装显卡驱动： [链接](https://www.cnblogs.com/myblog1993/p/9284071.html)

(8) grep -r "查询内容"  文件目录    #这样查询出来的包括文件名+内容

(9) dpkg -L package 查看安装包安装的信息(apt-get install)

(10) 在目录下匹配 find . |xargs grep -ni -s -i --color "xxxxxx"

(11) 终端terminal 输出到log中 在后面加上  >log.txt 2>&1

(12) 对数据集(或文件)创建文件关联 ln -s /home/user/data/VOC0712_trainval_lmdb trainval_lmdb (trainval_lmdb是当前目录下创建的文件夹，通往数据集)

(13) g++ 编译时连接caffe库　g++ main.cpp -I /home/user/wuzhe/caffe/include/

(14) 单个文件编译 g++ test.cpp -o test

(15) 历史命令查询 history |grep "xxxxx"

(16) 命令行挂载外部设备 

ls /dev/sd* 查看是否有设备 

mount /dev/sda1 /mnt 把U盘挂载到mnt上 (mount用于挂载Linux系统外的文件)





# git命令
(1) 拉取分支 git clone -b xxx(分支名) http:xxxxxxx

(2) git 更新代码到本地

查看远程代码版本 git remote -v

获取最新代码到本地(本地当前分支为branch，获取的远端的分支为origin/branch)

git fetch origin master  示例1：获取远端的origin/master分支

git fetch origin dev 示例2：获取远端的origin/dev分支

查看版本差异

git log -p master..origin/master 示例1：查看本地master与远端origin/master的版本差异

git log -p dev..origin/dev   示例2：查看本地dev与远端origin/dev的版本差异

合并最新代码到本地分支

git merge origin/master  示例1：合并远端分支origin/master到当前分支

git merge origin/dev 示例2：合并远端分支origin/dev到当前分支

(3) 提交代码到分支

 git status //命令用于显示工作目录和暂存区的状态
 
 git add . //命令用于将工作区中所有未跟踪或者修改的文件添加到暂存区,不包含删除的文件(注意最后的"."前面有个空格, .代表当前目录)
  
 git commit - m "xxx" //命令用于把暂存区的文件提交到本地 （xxx为本次提交代码的备注）
  
 git pull origin dev //命令用于远程master的代码下拉到本地分支dev,如果有冲突先解决冲突然后再重复 2 和3的步骤
  
 git push origin dev //命令用于把本地代码提交到远程分支
