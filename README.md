## AlibabaCloudACR
GitHub Actions / 阿里云 ACR 中转


### 1. 登录阿里云 Container Registry
```yml
docker login --username=exzhanhao crpi-tjpbhu7ev24zh1rq.cn-hangzhou.personal.cr.aliyuncs.com
```

### 2. 拉取镜像的格式：docker pull [Registry地址]/[命名空间]/[仓库名]:[镜像名]_[标签]


```yml
docker pull crpi-tjpbhu7ev24zh1rq.cn-hangzhou.personal.cr.aliyuncs.com/garendeng_zhanhao/james-hub:mysql_8.0
```
