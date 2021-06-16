
## 一. 文件
### 1. 创建文件夹
```Shell
mkdir "dirname"
```
### 2. 删除空文件夹
```Shell
rmdir "dirname"
```

### 3. 删除文件夹及以下的所有文件
```Shell
rm -fr ./path/file

r:recursion 递归
f:force     强行
```

### 4. 查看文件内容 concatenate
```shell
cat "path/filename"
```

### 5. 查看当前目录下的文件大小 
```shell
ls -lht           看文件大小
du -sh *          看文件大小
du -sh /home      看对应目录下文件大小 
```

## 二. 时间
### 1. 系统当时间
```shell
date
```

### 2. 日历
```shell
cal 
cal 1995
cal 12 1995
```

### 3. 系统程序执行时间
```shell
time
```
