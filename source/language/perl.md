# Perl

## One Liner
### 处理空行
```bash
perl -i  -n  -e 'print if /\S/' file
```
等价于 `awk`
```bash
sed -i  '/^$/d' file
```
