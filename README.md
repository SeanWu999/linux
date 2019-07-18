# linux命令

(1) sudo chmod -R 777 wuzhe/  解锁wuzhe下的权限，777是最大的

(2) python3 编译pyc python3 -m compileall -b .

(3) python2 编译pyc python -m compileall .

(4) lib****.so.10报错，用以下语句重置  sudo ldconfig /usr/local/cuda-10.0/lib64 （在使用编译后的caffe，openpose时出现的）
