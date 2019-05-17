# 国内镜像列表

## Docker Hub 镜像

- Docker 中国镜像：https://registry.docker-cn.com
- 开源社镜像：https://dockerhub.akscn.io

示例

```sh
docker pull registry.docker-cn.com/library/nginx
```

## GCR（Google Container Registry）镜像

- 开源社镜像：https://gcr.akscn.io/google_containers

示例

```sh
docker pull gcr.akscn.io/google_containers/hyperkube:v1.12.1
docker pull gcr.akscn.io/google_containers/pause-amd64:3.1
```

- Azure中国镜像：gcr.azk8s.cn/google_containers

示例

```sh
docker pull gcr.azk8s.cn/google_containers/pause-amd64:3.0
docker pull gcr.azk8s.cn/google_containers/kubedns-amd64:1.7
```

## Kubernetes RPM/DEB镜像

- [开源社镜像](http://mirror.azure.cn/kubernetes/packages/)

示例：

```sh
# Ubuntu
cat <<EOF >/etc/apt/sources.list.d/kubernetes.list
deb http://mirror.azure.cn/kubernetes/packages/apt/ kubernetes-xenial main
EOF
```

### Helm Charts 镜像

- Helm: http://mirror.azure.cn/kubernetes/helm/
- Stable Charts: http://mirror.azure.cn/kubernetes/charts/
- Incubator Charts: http://mirror.azure.cn/kubernetes/charts-incubator/

示例

```sh
helm repo add stable http://mirror.azure.cn/kubernetes/charts/
helm repo add incubator http://mirror.azure.cn/kubernetes/charts-incubator/
```

## 操作系统镜像

- [开源社开源镜像](http://mirror.azure.cn/)
- [网易开源镜像](https://mirrors.163.com/)

以 Ubuntu 18.04（Bionic）为例，修改 /etc/apt/sources.list 文件的内容为

```sh
deb http://azure.archive.ubuntu.com/ubuntu/ bionic main restricted universe multiverse
deb http://azure.archive.ubuntu.com/ubuntu/ bionic-security main restricted universe multiverse
deb http://azure.archive.ubuntu.com/ubuntu/ bionic-updates main restricted universe multiverse
deb http://azure.archive.ubuntu.com/ubuntu/ bionic-proposed main restricted universe multiverse
deb http://azure.archive.ubuntu.com/ubuntu/ bionic-backports main restricted universe multiverse
deb-src http://azure.archive.ubuntu.com/ubuntu/ bionic main restricted universe multiverse
deb-src http://azure.archive.ubuntu.com/ubuntu/ bionic-security main restricted universe multiverse
deb-src http://azure.archive.ubuntu.com/ubuntu/ bionic-updates main restricted universe multiverse
deb-src http://azure.archive.ubuntu.com/ubuntu/ bionic-proposed main restricted universe multiverse
deb-src http://azure.archive.ubuntu.com/ubuntu/ bionic-backports main restricted universe multiverse
```
