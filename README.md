# linux命令

(1) sudo chmod -R 777 wuzhe/  解锁wuzhe下的权限，777是最大的       chmod u+x filename 使文件有可执行权限

(2) python3 编译pyc python3 -m compileall -b .

(3) python2 编译pyc python -m compileall .

(4) lib****.so.10报错，用以下语句重置  sudo ldconfig /usr/local/cuda-10.0/lib64 （在使用编译后的caffe，openpose时出现的）

(5) grep Aug /var/log/messages 在文件 '/var/log/messages'中查找关键词"Aug" 

(6) ubuntu18 配置静态IP： '参考1' [website](https://blog.csdn.net/qq_34889607/article/details/82497405)，'参考2' [website](https://www.jianshu.com/p/2b401aa0052d)

(7) ubuntu16 安装显卡驱动： [链接](https://www.cnblogs.com/myblog1993/p/9284071.html)

(8) grep -r "查询内容"  文件目录    #这样查询出来的包括文件名+内容

（９） dpkg -L package 查看安装包安装的信息(apt-get install)

(10) 在目录下匹配 find . |xargs grep -ni -s -i --color "xxxxxx"

(11) 终端terminal 输出到log中 在后面加上  >log.txt 2>&1

(12) 对数据集(或文件)创建文件关联 ln -s /home/user/data/VOC0712_trainval_lmdb trainval_lmdb (trainval_lmdb是当前目录下创建的文件夹，通往数据集)

(13) g++ 编译时连接caffe库　g++ main.cpp -I /home/user/wuzhe/caffe/include/

(14) 单个文件编译 g++ test.cpp -o test
