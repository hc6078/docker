## docker常用命令

### 镜像命令

#### 1 拉取镜像

docker pull images

#### 2 查看镜像

docker images

#### 3 删除镜像(先删除运行这个镜像的容器在删除镜像)

docker rmi image_name



### 容器命令

#### 1 哪些容器在运行 

docker ps -a 

#### 2 容器进行启动

docker start container_id 

#### 3 容器进行重启

docker restart  container_id 

#### 4 容器进行停止

docker stop container_id 

#### 5 进入容器中

docker exec -it container_id /bin/bash 
docker attach container_id 

#### 6 运行容器中的镜像（第一次启动使用这个命令,主动stop后要用restart命令启动）

docker run -t -i container_id 	

#### 7 删除容器(先stop容器才能执行删除)

docker rm container_id 
