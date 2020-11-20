# K8S
## containerd
### 获取镜像
```bash
sudo ctr image pull <image>
```

### 镜像代理加速
```bash
sudo ctr image pull registry.aliyuncs.com/<image>
```

### 重命名镜像
```bash
sudo ctrl image tag <image1> <image2>
```

### 查看容器信息
```bash
sudo ctr c list
```

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

## deployment
K8S 通过创建 `Deployment` 对象来管理 `Pod` ， 但是在实际上部署的底层过程中是通过创建 `ReplicaSet` 来控制新老副本的数量，比如说升级应用，会新创建一个新的 `ReplicaSet` 控制新的 `ReplicaSet` 和 老的 `ReplicaSet` 的 `Pod` 数量来控制新老副本的的数量，从而实现滚动发布。
