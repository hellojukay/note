# K8S
## K3S
### 官方网站
https://docs.rancher.cn/

### 安装脚本
```bash
curl -sfL https://get.k3s.io | sh -
```
国内用户用下面这种安装方式:
```bash
curl -sfL http://rancher-mirror.cnrancher.com/k3s/k3s-install.sh | INSTALL_K3S_MIRROR=cn sh -
```
### 获取节点
```bash
k3s kubectl get nodes
```
### 查看命名空间
```bash
k3s kubectl get ns
```
### 查看 pod
```bash
k3s kubectl get pods
```
