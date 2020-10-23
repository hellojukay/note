# Gitlab Pipeline

## 跳过机器人提交
```bash
git push --option=ci.skip     # 需要 git 2.10+
git push  -o ci.skip          # 需要 git 2.18+ 猜测 -o 就是 --option 的简写
```
