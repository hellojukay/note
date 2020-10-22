# Linux

## envsubst
这个命令能够根据当前 `bash` 的环境变量来渲染文件
```bash
vim a.txt
# 内容如下
$HOME
```
```bash
cat a.txt
# 内容如下
$HOME
```
如果将文件内容发送给 `envsubst` 命令，内容就会被环境变量替换
```bash
cat a.txt | envsubt
# 内容如下
/home/hellojukay
```
或者
```bash
envsubt < a.txt
# 内容如下
/home/hellojukay
```

## when-changed
when-changed 是一个监控文件的工具，当文件发生改变以后，能自动触发某些预定义的操作。常用来做自动编译代码，实时预览。
```
https://github.com/joh/when-changed
```
安装
```bash
pip install when-changed -i https://mirrors.aliyun.com/pypi/simple/
```
使用方式
```
when-changed <dir or files> -c <your command>
```
具体可以参考：
```
https://gaopinghuang0.github.io/2018/05/23/when-changed-usage
```

