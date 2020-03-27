# docker常见命令


```
docker info //查看docker信息
docker inspect //容器名称或 id
docker ps //查看当前运行中的容器
docker ps -a //查看所有运行过的容器
docker inspect containerId(容器ID或容器名)//查看对应容器的具体配置信息
docker port containerId //查看对应容器端口映射
docker run --name containerName -it -p 80:80 -d // --name是为容器取一个别名，-p 80:80是端口映射，将宿主机的80端口映射到容器的80端口上，-d是指后台运行容器，即容器启动后不会停止，-it是-i 和-t的合并，以交互模式运行容器。
docker images //查看所有镜像
docker exec -it containerName /bin/bash //进入已启动的容器内，新启一个进程，执行命令。
docker stop containerName // 停止一个容器
docker start -i containerName //重启启动一个运行过的容器
docker rm containerName //移除一个容器
docker run image_name apt-get install -y app_name  //在容器中安装新的程序 
```

# IP

- 172.18.39.113


# scrapy-splash

- 命令

```
    docker run -d -p 8050:8050 scrapinghub/splash  //启动命令
    docker run -p 5023:5023 -p 8050:8050 -p 8051:8051 scrapinghub/splash  //8050(http),8051(https),5023 (telnet)
```

#

1688搜索引发的链接：https://s.1688.com/selloffer/offer_search.htm?keywords=%B4%BA%CF%C4Ůװ&n=y&netType=16&beginPage=1#sm-filtbar

http://search.1688.com/service/marketOfferResultViewService?keywords=%B4%BA%CF%C4Ůװ&n=y&netType=16&beginPage=1&async=true&asyncCount=20&pageSize=60&requestId=1825012230015853001734055000557&startIndex=20