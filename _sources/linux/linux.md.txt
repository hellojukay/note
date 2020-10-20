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
