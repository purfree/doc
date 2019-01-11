### 查找镜像
docker search name
### 下载镜像
docker pull name
### 查看运行的容器挂载的目录
docker inspect container_name | grep Mounts -A 20
### 删除容器
docker rm $(docker ps -aq)
### 查看容器IP
docker inspect --format '{{ .NetworkSettings.IPAddress }}' \<container-ID>  
或  
docker inspect \<container id>  