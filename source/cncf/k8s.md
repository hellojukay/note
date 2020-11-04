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


