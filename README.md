
设置国内docker image 仓库地址

cat /etc/docker/daemon.json 
{
"registry-mirrors": ["https://registry.docker-cn.com"]
}



0 搜索镜像
  docker search
  docker pull mysql  
  docker info
  docker stats  
1 docker images

2 docker ps -a -l

3 docker build -t pez1420/javavul:test . --rm=true
-t选择指定生成镜像的用户名，仓库名和tag
--rm=true指定在生成镜像过程中删除中间产生的临时容器。

4 docker images pez1420/javavul
查看新产生的镜像

5 运行镜像
	docker run -d -p 8090:8080 5207
		-p指定主机80端口与容器8080端口进行绑定
		-d 指定容器运行后与当前tty分离，后台运行
		5207是镜像的ID前4位。

6 停用全部运行中的容器
docker stop $(docker ps -q)
docker stop 2882c14cefa9(容器ID)

7 删除所有容器
docker rm $(docker ps -aq)

8 进入容器
docker inspect 来查看该容器的详细信息

docker exec -it 8f1b89183df5 /bin/sh   
  8f1b89183df5为容器ID  /bin/sh需要执行的命令
	-d :分离模式: 在后台运行
	-i :即使没有附加也保持STDIN 打开
	-t :分配一个伪终端
  
共享文件目录:
cd /mnt/hgfs/


8 删除images，通过image的id来指定删除谁
docker rmi <image id>

