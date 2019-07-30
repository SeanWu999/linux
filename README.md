# linux命令

sudo chmod -R 777 wuzhe/  解锁wuzhe下的权限，777是最大的

python3 编译pyc python3 -m compileall -b .

python2 编译pyc python -m compileall .

lib****.so.10报错，用以下语句重置  sudo ldconfig /usr/local/cuda-10.0/lib64 （在使用编译后的caffe，openpose时出现的）

grep Aug /var/log/messages 在文件 '/var/log/messages'中查找关键词"Aug" 
