# 查找
```
# 查找所有名称为src的文件夹
find . -name src -type d
# 查找所有文件夹路径中包含test的python文件
find . -path '**/test/**/*.py' -type f
# 查找前一天修改的所有文件
find . -mtime -1
# 查找所有大小在500k至10M的tar.gz文件
find . -size +500k -size -10M -name '*.tar.gz'
```

# 磁盘
```
# 查看文件信息
df -h

# 挂载内存盘
mount -t tmpfs -o size=5G tmpfs /tmp/xxx

# 取消文件挂载
umout /tmp/xxx

# 设置共享内存大小
mount -o remount,size=64g /dev/shm

# 挂载磁盘
mount /dev/vdc /data

# 查看已有磁盘
fdisk -l

# 磁盘格式化
mkfs.ext4 /dev/vdc
```

# 网络
```
netstat -tunlp
```

# 进程查看
```
```

# 压缩
```
tar cvf xxx.tar xxx/
tar zcvf xxx.tar.gz xxx/
tar xcf xxx.tar
tar zxcf xxx.tar.gz

```
