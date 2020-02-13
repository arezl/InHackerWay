# shell

```bash
# 使用shell来执行
$ sh hello.sh
# 使用bash来执行
$ bash hello.sh
使用.来执行
$ . ./hello.sh
使用source来执行
$ source hello.sh
还可以赋予脚本所有者执行权限，允许该用户执行该脚本
$ chmod u+rx hello.sh
$  ./hello.sh
locate bash ,find / -name bash 2>/dev/null 或 whereis bash
path =`pwd` 或者$(pwd)
echo $path
> 这个符号是重定向,执行以下代码，就会在当前目录下生成一个my.txt
垃圾桶（/dev/null）
```

 

less 查看并搜索shiyanlou

```bash
less shiyanlou.log
/shiyanlou
```

ps 查看进程信息并通过 less 分页显示，可以使用如下命令

```
ps -f | less
```

cat 命令功能：用于显示整个文件的内容，因为单独使用没有翻页功能，所以经常和 more 命令搭配使用，cat 命令还有一个可以将数个文件合并成一个文件的功能。

head 

head -n 5 shiyanlou.log

tail 命令主要用于显示指定文件末尾内容。常用查看日志文件。

tail -n 5 shiyanlou.log

 tail 命令的 -f 选项可以即时输出文件变化后追加的内容，tail -f filename 会把 filename 里最尾部的内容显示在屏幕上，并且不断刷新，使你看到最新的文件内容

 jobs 命令可以查看正在后台运行的任务。kill 命令可以杀死一个任务，但要使用任务的 pid。任务的 pid 可以通过 ps 命令查看获得，然后使用kill -9 任务pid就可以将这个后台进程杀死。