# linux命令

(1) sudo chmod -R 777 wuzhe/  解锁wuzhe下的权限，777是最大的

(2) python3 编译pyc python3 -m compileall -b .

(3) python2 编译pyc python -m compileall .

(4) lib****.so.10报错，用以下语句重置  sudo ldconfig /usr/local/cuda-10.0/lib64 （在使用编译后的caffe，openpose时出现的）

(5) grep Aug /var/log/messages 在文件 '/var/log/messages'中查找关键词"Aug" 

(6) ubuntu18 配置静态IP： '参考1' [website](https://blog.csdn.net/qq_34889607/article/details/824974)，'参考2' [website](https://www.jianshu.com/p/2b401aa0052d)
