## 🛠️ 使用方法
在 Actions 页面点击 Docker Image Sync to ACR。

点击 Run workflow。

输入你想同步的 Docker Hub 镜像名（例如：mysql:8.0 或 1panel/openresty:latest）。

等待同步完成后，直接在服务器执行页面生成的 docker pull 命令。

## 🔒 安全配置 (Secrets)
需要在仓库设置中配置以下密钥：

ACR_USERNAME: 阿里云容器镜像仓库登录名。

ACR_PASSWORD: 阿里云容器镜像仓库固定密码。

ALIBABA_CLOUD_ACCESS_KEY_ID: 阿里云 AK（用于 API 同步列表）。

ALIBABA_CLOUD_ACCESS_KEY_SECRET: 阿里云 SK。


##  拉取镜像操作
### 1. 登录阿里云 Container Registry
```yml
docker login --username=exzhanhao crpi-tjpbhu7ev24zh1rq.cn-hangzhou.personal.cr.aliyuncs.com
```

### 2. 拉取镜像的格式：docker pull [Registry地址]/[命名空间]/[仓库名]:[镜像名]_[标签]

```yml
docker pull crpi-tjpbhu7ev24zh1rq.cn-hangzhou.personal.cr.aliyuncs.com/garendeng_zhanhao/james-hub:mysql_8.0
```
