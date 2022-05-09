## 安装 Docker 环境

下载安装相关系统发行版 Docker
[https://www.docker.com/get-started/](https://www.docker.com/get-started/)

## 基于 Minio 自建对象存储

```shell
docker run \
  -p 9000:9000 \
  -p 9001:9001 \
  -e "MINIO_ROOT_USER=minioadmin" \
  -e "MINIO_ROOT_PASSWORD=minioadmin" \
  quay.io/minio/minio server /data --console-address ":9001"
```

访问 http://127.0.0.1:9001/ 

登录账户名和密码默认为 minioadmin

登录进去后点击创建 Busket 

<img width="1725" alt="image" src="https://user-images.githubusercontent.com/40495740/167343233-202e18fb-6172-4230-868b-25d6613452fd.png">
