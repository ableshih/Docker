# Docker

# Docker

Win11 / 10 上用免费的Docker架设WordPress
https://www.youtube.com/watch?v=Tx0Nr0IHEKY

安裝 Install Docker Desktop on Windows
https://docs.docker.com/desktop/windows/install/
'Docker Desktop Installer.exe'



## 在 Windows 上進行 Docker 遠端開發的概觀
https://docs.microsoft.com/zh-tw/windows/dev-environment/docker/overview


Docker Engine

* Windows 
    Windows Hyper-V
    WSL
* Linux
* iOS
    VB
    
```

```


docker quickstar teminal
```
Creating CA: C:\Users\LC55-14C\.docker\machine\certs\ca.pem
Creating client certificate: C:\Users\LC55-14C\.docker\machine\certs\cert.pem
Running pre-create checks...
Error with pre-create check: "This computer doesn't have VT-X/AMD-v enabled. Enabling it in the BIOS is mandatory"
Looks like something went wrong in step ´Checking if machine default exists´... Press any key to continue...
```



```
Windows PowerShell
著作權（C） Microsoft Corporation。保留擁有權利。

安裝最新的 PowerShell 以取得新功能和改進功能！https://aka.ms/PSWindows

PS C:\Windows\system32> docker run hello-world
docker: error during connect: In the default daemon configuration on Windows, the docker client must be run with elevated privileges to connect.: Post "http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.24/containers/create": open //./pipe/docker_engine: The system cannot find the file specified.
See 'docker run --help'.
PS C:\Windows\system32> docker run hello-world
docker: error during connect: In the default daemon configuration on Windows, the docker client must be run with elevated privileges to connect.: Post "http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.24/containers/create": open //./pipe/docker_engine: The system cannot find the file specified.
See 'docker run --help'.
PS C:\Windows\system32> "C:\Program Files\Docker\Docker\DockerCli.exe" -SwitchDaemon
位於 線路:1 字元:48
+ "C:\Program Files\Docker\Docker\DockerCli.exe" -SwitchDaemon
+                                                ~~~~~~~~~~~~~
運算式或陳述式中有未預期的 '-SwitchDaemon' 語彙基元。
    + CategoryInfo          : ParserError: (:) [], ParentContainsErrorRecordException
    + FullyQualifiedErrorId : UnexpectedToken

PS C:\Windows\system32> docker run hello-world
docker: error during connect: In the default daemon configuration on Windows, the docker client must be run with elevated privileges to connect.: Post "http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.24/containers/create": open //./pipe/docker_engine: The system cannot find the file specified.
See 'docker run --help'.
PS C:\Windows\system32>

```


```
Microsoft Windows [版本 10.0.22000.376]
(c) Microsoft Corporation. 著作權所有，並保留一切權利。

C:\Windows\system32>docker run hello-world
docker: error during connect: In the default daemon configuration on Windows, the docker client must be run with elevated privileges to connect.: Post "http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.24/containers/create": open //./pipe/docker_engine: The system cannot find the file specified.
See 'docker run --help'.

C:\Windows\system32>docker pull hello-world
Using default tag: latest
error during connect: In the default daemon configuration on Windows, the docker client must be run with elevated privileges to connect.: Post "http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.24/images/create?fromImage=hello-world&tag=latest": open //./pipe/docker_engine: The system cannot find the file specified.

C:\Windows\system32>docker pull ableshih/hello-world
Using default tag: latest
error during connect: In the default daemon configuration on Windows, the docker client must be run with elevated privileges to connect.: Post "http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.24/images/create?fromImage=ableshih%2Fhello-world&tag=latest": open //./pipe/docker_engine: The system cannot find the file specified.

C:\Windows\system32>docker run hello-world
docker: error during connect: In the default daemon configuration on Windows, the docker client must be run with elevated privileges to connect.: Post "http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.24/containers/create": open //./pipe/docker_engine: The system cannot find the file specified.
See 'docker run --help'.

C:\Windows\system32>"C:\Program Files\Docker\Docker\DockerCli.exe" -SwitchDaemon

C:\Windows\system32>docker run hello-world
docker: error during connect: In the default daemon configuration on Windows, the docker client must be run with elevated privileges to connect.: Post "http://%2F%2F.%2Fpipe%2Fdocker_engine/v1.24/containers/create": open //./pipe/docker_engine: The system cannot find the file specified.
See 'docker run --help'.

C:\Windows\system32>
```


https://docs.docker.com/engine/reference/commandline/docker/

## 安装 
https://www.runoob.com/docker/docker-build-command.html
    Ubuntu
    Debian 
    CentOS 
    Windows 
    MacOS
https://docs.docker.com/desktop/windows/install/
WSL 2 backend
https://hub.docker.com/editions/community/docker-ce-desktop-windows
1. 下載 
    https://desktop.docker.com/win/stable/amd64/Docker%20Desktop%20Installer.exe
2. 安裝 (不用重開機)
3. 執行
    Open a command-line terminal like PowerShell, and try out some Docker commands!

    Run docker --version to check the version.

    Run docker run hello-world to verify that Docker can pull and run images.
```
C:\Users\LC55-14C>docker --version
Docker version 20.10.11, build dea9396

C:\Users\LC55-14C>
```

5. 



## 流程
* 1. 建立自己的 code
* 2. 寫入Dockerfile
* 3. 建立images
* 4. 定義services
* 5. run containers
* 6. test My code
* 7. git push

## 網站資源
* Docker 教程
https://www.runoob.com/docker/docker-tutorial.html
* Docker 初學筆記 - 基本指令操作教學
https://blog.longwin.com.tw/2017/01/docker-learn-initial-command-cheat-sheet-2017/
* Docker CLI
https://docs.docker.com/engine/reference/commandline/docker/
* 用30天來介紹和使用 Docker
https://ithelp.ithome.com.tw/users/20103456/ironman/1320
* Docker學習筆記
https://peihsinsu.gitbooks.io/docker-note-book/
* Get started with Docker for Windows
https://docs.docker.com/desktop/windows/
* Docker初體驗
https://peihsinsu.gitbooks.io/docker-note-book/content/install-docker.html


## Docker 10大指令
* 抓取網路上的 image
https://www.youtube.com/watch?v=sxuynZ3wIa8
$ docker pull alpine:latest
** 抓 alpine 最新版 Alpine Linux 是一套極小安全又簡單的作業系統
$ docker images # 查看是否安裝成功
$ docker run alpine # 啟動 alpine
$ docker run -d -it alpine /bin/sh # -d 背景執行
$ docker container ls # 列出執行的的 container ID
$ docker exec -it 找到的ID /bin/sh
進入之後輸入 exit 離開
$ clear # 是 linux 清畫面指令
$ docker container stop 要停止的ID (停止運行但還在)
$ docker container rm 要停止的ID (停止運行清楚)
$ docker rmi alpine (刪除 alpine image)

vi Dockerfile

FROM alpine:latest
RUN apk --update add apache2
RUN rm -rf /var/cache/apk/*
ENTRYPOINT ["httpd", "-D", "FOREGROUND"]

docker build -t myimage . (將Dockerfile 打包成image )


## 容器连接
创建了一个 python 应用的容器
```
docker run -d -P training/webapp python app.py
docker ps
docker run -d -p 127.0.0.1:5001:5000 training/webapp python app.py
```


## docker image 建造與使用
Dockerfile -> docker build -> Docker Image
```

```

Dockerfile->Docker Image->Container->docker commit->Docker Image
```

```
container 轉 image
## 建造
### container
#### Docker圖解教學 將Container變成Docker Image
https://www.youtube.com/watch?v=1wfgS31LcgQ
```
$ ls (查看 Dockerfile)
$ cat Dockerfile (查看 Dockerfile 內容)
$ docker build -t 帳號名/myimage .
$ docker images (看到新 帳號名/myimage)
$ docker run -d -p 8080:80 帳號名/myimage (把新的 image 跑起來)
$ docker container ls ()
$ echo $(docker-machine ip) (查看ip addr.)
複製 ip 貼到瀏覽器 :8080 (可看到已跑起來的網頁)
$ docker container ls (查找 ID)
$ docker exec -it ID /bin/sh (進到 container 裡)
$ ls (會看到 index.html)
$ cat index.html (查看 index.html 內容)
$ echo "要加入顯示內容" >> index.html (加入新內容 index.html 裡)
$ cat index.html (查看 index.html 內容)
回到 瀏覽器 重整 (可看到 index.html 已加入新內容)
$ exit
把 container 轉成 image
$ docker commit containerID dockerHUB帳號名/新image名稱
$ docker images (可看到新建的image)
$ docker ls (列)
$ docker stop ID (停)
$ docker rm ID (清)
$ docker images
$ docker run -d -p 8080:80 帳號名/新的image
$ docker container ls
$ echo $(docker-machine ip) 
```

    從網路
### Dockerfile -> image #用文字檔
* Dockerfile -> docker build -> Docker Image
```
$ vi Dockerfile

FROM alpine:latest
RUN apk --update add apache2
RUN rm -rf /var/cache/apk/*
ENTRYPOINT ["httpd", "-D", "FOREGROUND"]

$ docker build -t myimage . (將Dockerfile 打包成image )
```

## 指令
https://docs.docker.com/engine/reference/commandline/docker/
### 0. docker -v 掛載點
    * version 

### 1. docker attach	
    Attach local standard input, output, and error streams to a running container 
    將本地標準輸入、輸出和錯誤流附加到正在運行的容器
    $ docker attach [OPTIONS] CONTAINER
    * Docker 進入(Attach) Container
    docker attach hash-id
    docker attach 1e560fca3906

### 2. docker build	
    Build an image from a Dockerfile 
    從 Dockerfile 構建鏡像
    $ docker build [OPTIONS] PATH | URL | -
    $ docker build github.com/creack/docker-firefox

### 3. docker builder	
    Manage builds 管理構建
    $ docker builder COMMAND

### 4. docker checkpoint	
    Manage checkpoints 管理檢查點
    $ docker checkpoint COMMAND

### 5. docker commit	
    Create a new image from a container’s changes 
    從容器的更改中創建新圖像
    $ docker commit [OPTIONS] CONTAINER [REPOSITORY[:TAG]]

### 6. docker config	
    Manage Docker configs 管理 Docker 配置
    $ docker config COMMAND

### 7. docker container	
    Manage containers 管理容器
    $ docker container COMMAND

### 8. docker context	
    Manage contexts 管理上下文
    $ docker context COMMAND

### 9. docker cp	
    Copy files/folders between a container and the local filesystem 
    在容器和本地文件系統之間複製文件/文件夾
    $ docker cp [OPTIONS] CONTAINER:SRC_PATH DEST_PATH|-

### 10. docker create	
    Create a new container 創建一個新容器
    $ docker create [OPTIONS] IMAGE [COMMAND] [ARG...]
    $ docker create -v /home/docker:/docker --name docker ubuntu

### 11. docker diff	
    Inspect changes to files or directories on a container’s filesystem 
    檢查容器文件系統上文件或目錄的更改
    $ docker diff CONTAINER
    $ docker diff 1fdfd1f54c1b

### 12. docker events	
    Get real time events from the server 
    從服務器獲取實時事件
    $ docker events [OPTIONS]

### 13. docker exec	
    Run a command in a running container 
    在正在運行的容器中運行命令
    $ docker exec [OPTIONS] CONTAINER COMMAND [ARG...]
    $ docker exec -d ubuntu_bash touch /tmp/execWorks
    * Docker 執行 Container
    docker exec hash-id /sbin/ifconfig
    docker exec -it 243c32535da7 /bin/bash

### 14. docker export	
    Export a container’s filesystem as a tar archive 
    將容器的文件系統導出為 tar 存檔
    $ docker export [OPTIONS] CONTAINER
    $ docker export --output="latest.tar" red_panda
    docker export 1e560fca3906 > ubuntu.tar

### 15. docker history	
    Show the history of an image 
    顯示圖像的歷史
    $ docker history [OPTIONS] IMAGE
    $ docker history docker

### 16. docker image	
    Manage images 管理圖像
    $ docker image COMMAND
    * 映像檔 Image
    * Docker 執行 Image
    * Docker 掛載目錄進入 Container

### 17. docker images	
    List images 列出圖像
    $ docker images [OPTIONS] [REPOSITORY[:TAG]]
    $ docker images java
    * Docker 列出 Local Images
    docker images

### 18. docker import	
    Import the contents from a tarball to create a filesystem image 
    從 tarball 導入內容以創建文件系統映像
    $ docker import [OPTIONS] file|URL|- [REPOSITORY[:TAG]]
    $ docker import https://example.com/exampleimage.tgz
    docker import http://example.com/exampleimage.tgz example/imagerepo

### 19. docker info	
    Display system-wide information 
    顯示系統範圍的信息
    $ docker info [OPTIONS]
    docker info

### 20. docker inspect	
    Return low-level information on Docker objects 
    返回有關 Docker 對象的低級信息
    $ docker inspect [OPTIONS] NAME|ID [NAME|ID...]
    $ docker inspect --format='{{.Config.Image}}' $INSTANCE_ID

### 21. docker kill	
    Kill one or more running containers 
    殺死一個或多個正在運行的容器
    $ docker kill [OPTIONS] CONTAINER [CONTAINER...]
    $ docker kill my_container
    $ docker kill --signal=SIGHUP my_container
    $ docker kill --signal=HUP my_container
    $ docker kill --signal=1 my_container

### 22. docker load	
    Load an image from a tar archive or STDIN 
    從 tar 存檔或 STDIN 加載圖像
    $ docker load [OPTIONS]
    $ docker load --input fedora.tar

### 23. docker login	
    Log in to a Docker registry 
    登錄到 Docker 註冊表
    $ docker login [OPTIONS] [SERVER]
    $ docker login localhost:8080
    docker login
    
### 24. docker logout	
    Log out from a Docker registry 
    從 Docker 註冊表中註銷
    $ docker logout [SERVER]
    $ docker logout localhost:8080
    docker logout

### 25. docker logs	
    Fetch the logs of a container 獲取容器的日誌
    $ docker logs [OPTIONS] CONTAINER
    $ docker logs -f --until=2s test
    docker logs -f bf08b7f2cd89
    docker logs hash-id # * Docker 列出 Logs

### 26. docker manifest	
    Manage Docker image manifests and manifest lists 
    管理 Docker 鏡像清單和清單列表
    $ docker manifest COMMAND COMMAND
    $ docker manifest inspect --help

### 27. docker network	
    Manage networks 管理網絡
    $ docker network COMMAND

### 28. docker node	
    Manage Swarm nodes 管理 Swarm 節點
    $ docker node COMMAND

### 29. docker pause	
    Pause all processes within one or more containers 
    暫停一個或多個容器內的所有進程
    $ docker pause CONTAINER [CONTAINER...]
    $ docker pause my_container

### 30. docker plugin	
    Manage plugins 管理插件
    $ docker plugin COMMAND

### 31. docker port	
    List port mappings or a specific mapping for the container 
    列出容器的端口映射或特定映射
    $ docker port CONTAINER [PRIVATE_PORT[/PROTO]]
    $ docker port test 7890/udp
    docker port bf08b7f2cd89

### 32. docker ps	
    List containers 列出容器
    $ docker ps [OPTIONS]
    $ docker ps --filter "label=color"
    * Docker 列出 Container
    docker ps # 還在執行中的 Container，可以看到詳細 hash id
    docker ps -a # 執行、停止的 Container 都列出來
    docker ps -a
    docker ps

### 33. docker pull	
    Pull an image or a repository from a registry 
    從註冊表中提取圖像或存儲庫
    $ docker pull [OPTIONS] NAME[:TAG|@DIGEST]
    $ docker pull debian
    docker pull ubuntu
    docker pull ubuntu
    docker pull httpd
    docker pull ubuntu:13.10
    docker pull training/webapp

### 34. docker push	
    Push an image or a repository to a registry 
    將圖像或存儲庫推送到註冊表
    $ docker push [OPTIONS] NAME[:TAG]

### 35. docker rename	
    Rename a container 重命名容器
    $ docker rename CONTAINER NEW_NAME
    $ docker rename my_container my_new_container

### 36. docker restart	
    Restart one or more containers 
    重啟一個或多個容器
    $ docker restart [OPTIONS] CONTAINER [CONTAINER...]
    $ docker restart my_container
    docker restart <容器 ID>

### 37. docker rm	
    Remove one or more containers 移除一個或多個容器
    $ docker rm [OPTIONS] CONTAINER [CONTAINER...]
    $ docker rm --link /webapp/redis
    docker rm -f hash-id # 強置刪除
    docker rm -f 1e560fca3906
    docker rm wizardly_chandrasekhar
    * Docker 刪除 Container

### 38. docker rmi	
    Remove one or more images 移除一張或多張圖片
    $ docker rmi [OPTIONS] IMAGE [IMAGE...]
    $ docker rmi test1:latest
    * Docker 刪除 Images
    docker rmi image-id
    docker rmi -f image-id # 強置刪除    
    docker rmi hello-world

### 39. docker run	
    Run a command in a new container 在新容器中運行命令
    $ docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
    $ docker run --name test -it debian
    docker run -d debian:jessie
    docker run -d --name xxx -p 80:80 -p 3306:3306 -v /mnt/xxx:/mnt debian:jessie
    docker run -v myvol:/data # Container start 就 Mount 此 volume
    docker run -d -P training/webapp python app.py
    docker run ubuntu:15.10 /bin/echo "Hello world"
    docker run -itd --name ubuntu-test ubuntu /bin/bash
    docker run -it ubuntu /bin/bash
    docker run -t -i ubuntu:15.10 /bin/bash
    docker run httpd

### 40. docker save	
    Save one or more images to a tar archive (streamed to STDOUT by default) 
    將一個或多個圖像保存到 tar 存檔（默認流式傳輸到 STDOUT）
    $ docker save [OPTIONS] IMAGE [IMAGE...]
    $ docker save busybox > busybox.tar
    $ docker save -o ubuntu.tar ubuntu:lucid ubuntu:saucy

### 41. docker search	
    Search the Docker Hub for images 在 Docker Hub 中搜索圖像
    $ docker search [OPTIONS] TERM
    $ docker search busybox
    $ docker search --filter stars=3 busybox
    docker search nginx
    docker search httpd
    docker search ubuntu

### 42. docker secret	
    Manage Docker secrets 管理 Docker 機密
    $ docker secret COMMAND

### 43. docker service	
    Manage services 管理服務
    $ docker service COMMAND

### 44. docker stack	
    Manage Docker stacks 管理 Docker 堆棧
    $ docker stack [OPTIONS] COMMAND

### 45. docker start	
    Start one or more stopped containers 啟動一個或多個停止的容器
    $ docker start [OPTIONS] CONTAINER [CONTAINER...]
    $ docker start my_container
    * Docker 啟動 Image 產生 Container
    docker start hash-id
    docker start b750bbbcfd88

### 46. docker stats	
    Display a live stream of container(s) resource usage statistics 
    顯示容器資源使用統計的實時流
    $ docker stats [OPTIONS] [CONTAINER...]
    $ docker stats awesome_brattain 67b2525d8ad1
    docker stats --help

### 47. docker stop	
    Stop one or more running containers 
    停止一個或多個正在運行的容器
    $ docker stop [OPTIONS] CONTAINER [CONTAINER...]
    $ docker stop my_container
    * Docker 暫停 Image
    docker stop hash-id
    docker stop <容器 ID>
    
### 48. docker swarm	
    Manage Swarm 管理群
    $ docker swarm COMMAND

### 49. docker system	
    Manage Docker 管理 Docker
    $ docker system COMMAND

### 50. docker tag	
    Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE 
    創建一個引用 SOURCE_IMAGE 的標記 TARGET_IMAGE
    $ docker tag SOURCE_IMAGE[:TAG] TARGET_IMAGE[:TAG]
    $ docker tag httpd fedora/httpd:version1.0

### 51. docker top	
    Display the running processes of a container 顯示容器的運行進程
    $ docker top CONTAINER [ps OPTIONS]

### 52. docker trust	
    Manage trust on Docker images 管理對 Docker 映像的信任
    $ docker trust COMMAND

### 53. docker unpause	
    Unpause all processes within one or more containers 
    取消暫停一個或多個容器中的所有進程
    $ docker unpause CONTAINER [CONTAINER...]
    $ docker unpause my_container

### 54. docker update	
    Update configuration of one or more containers 
    更新一個或多個容器的配置
    $ docker update [OPTIONS] CONTAINER [CONTAINER...]
    $ docker update --cpu-shares 512 abebf7571666

### 55. docker version	
    Show the Docker version information 
    顯示 Docker 版本信息
    $ docker version [OPTIONS]
    $ docker version --format '{{.Server.Version}}'
    $ docker version --format '{{json .}}'
    $ docker version

### 56. docker volume	
    Manage volumes 管理卷
    $ docker volume COMMAND COMMAND
    * Docker 產生、操作 Volumes
    docker volume create --name myvol # 建立 local volume

### 57. docker wait	
    Block until one or more containers stop, then print their exit codes 
    阻塞直到一個或多個容器停止，然後打印它們的退出代碼
    $ docker wait CONTAINER [CONTAINER...]
    $ docker wait my_container




```

To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

shih@DESKTOP-EVK789N:~$ wsl --list

Command 'wsl' not found, but can be installed with:

sudo apt install wsl

shih@DESKTOP-EVK789N:~$ sudo apt-get update
[sudo] password for shih:
Get:1 http://archive.ubuntu.com/ubuntu focal InRelease [265 kB]
Get:2 http://security.ubuntu.com/ubuntu focal-security InRelease [114 kB]
Get:3 http://security.ubuntu.com/ubuntu focal-security/main amd64 Packages [1135 kB]
Get:4 http://archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]
Get:5 http://archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]
Get:6 http://archive.ubuntu.com/ubuntu focal/main amd64 Packages [970 kB]
Get:7 http://security.ubuntu.com/ubuntu focal-security/main Translation-en [205 kB]
Get:8 http://security.ubuntu.com/ubuntu focal-security/main amd64 c-n-f Metadata [9104 B]
Get:9 http://security.ubuntu.com/ubuntu focal-security/restricted amd64 Packages [643 kB]
Get:10 http://security.ubuntu.com/ubuntu focal-security/restricted Translation-en [91.7 kB]
Get:11 http://security.ubuntu.com/ubuntu focal-security/restricted amd64 c-n-f Metadata [536 B]
Get:12 http://archive.ubuntu.com/ubuntu focal/main Translation-en [506 kB]
Get:13 http://security.ubuntu.com/ubuntu focal-security/universe amd64 Packages [675 kB]
Get:14 http://archive.ubuntu.com/ubuntu focal/main amd64 c-n-f Metadata [29.5 kB]
Get:15 http://archive.ubuntu.com/ubuntu focal/universe amd64 Packages [8628 kB]
Get:16 http://security.ubuntu.com/ubuntu focal-security/universe Translation-en [115 kB]
Get:17 http://security.ubuntu.com/ubuntu focal-security/universe amd64 c-n-f Metadata [13.0 kB]
Get:18 http://security.ubuntu.com/ubuntu focal-security/multiverse amd64 Packages [21.8 kB]
Get:19 http://security.ubuntu.com/ubuntu focal-security/multiverse Translation-en [4948 B]
Get:20 http://security.ubuntu.com/ubuntu focal-security/multiverse amd64 c-n-f Metadata [536 B]
Get:21 http://archive.ubuntu.com/ubuntu focal/universe Translation-en [5124 kB]
Get:22 http://archive.ubuntu.com/ubuntu focal/universe amd64 c-n-f Metadata [265 kB]
Get:23 http://archive.ubuntu.com/ubuntu focal/multiverse amd64 Packages [144 kB]
Get:24 http://archive.ubuntu.com/ubuntu focal/multiverse Translation-en [104 kB]
Get:25 http://archive.ubuntu.com/ubuntu focal/multiverse amd64 c-n-f Metadata [9136 B]
Get:26 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 Packages [1469 kB]
Get:27 http://archive.ubuntu.com/ubuntu focal-updates/main Translation-en [291 kB]
Get:28 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 c-n-f Metadata [14.7 kB]
Get:29 http://archive.ubuntu.com/ubuntu focal-updates/restricted amd64 Packages [694 kB]
Get:30 http://archive.ubuntu.com/ubuntu focal-updates/restricted Translation-en [99.0 kB]
Get:31 http://archive.ubuntu.com/ubuntu focal-updates/restricted amd64 c-n-f Metadata [532 B]
Get:32 http://archive.ubuntu.com/ubuntu focal-updates/universe amd64 Packages [892 kB]
Get:33 http://archive.ubuntu.com/ubuntu focal-updates/universe Translation-en [196 kB]
Get:34 http://archive.ubuntu.com/ubuntu focal-updates/universe amd64 c-n-f Metadata [19.9 kB]
Get:35 http://archive.ubuntu.com/ubuntu focal-updates/multiverse amd64 Packages [24.8 kB]
Get:36 http://archive.ubuntu.com/ubuntu focal-updates/multiverse Translation-en [6928 B]
Get:37 http://archive.ubuntu.com/ubuntu focal-updates/multiverse amd64 c-n-f Metadata [620 B]
Get:38 http://archive.ubuntu.com/ubuntu focal-backports/main amd64 Packages [42.0 kB]
Get:39 http://archive.ubuntu.com/ubuntu focal-backports/main Translation-en [10.0 kB]
Get:40 http://archive.ubuntu.com/ubuntu focal-backports/main amd64 c-n-f Metadata [864 B]
Get:41 http://archive.ubuntu.com/ubuntu focal-backports/restricted amd64 c-n-f Metadata [116 B]
Get:42 http://archive.ubuntu.com/ubuntu focal-backports/universe amd64 Packages [19.5 kB]
Get:43 http://archive.ubuntu.com/ubuntu focal-backports/universe Translation-en [13.4 kB]
Get:44 http://archive.ubuntu.com/ubuntu focal-backports/universe amd64 c-n-f Metadata [672 B]
Get:45 http://archive.ubuntu.com/ubuntu focal-backports/multiverse amd64 c-n-f Metadata [116 B]
Fetched 23.1 MB in 8s (2986 kB/s)
Reading package lists... Done
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce docker-ce-cli containerd.io
Reading package lists... Done
Building dependency tree
Reading state information... Done
Package docker-ce is not available, but is referred to by another package.
This may mean that the package is missing, has been obsoleted, or
is only available from another source

E: Package 'docker-ce' has no installation candidate
E: Unable to locate package docker-ce-cli
E: Unable to locate package containerd.io
E: Couldn't find any package by glob 'containerd.io'
E: Couldn't find any package by regex 'containerd.io'
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce docker-ce-cli
Reading package lists... Done
Building dependency tree
Reading state information... Done
Package docker-ce is not available, but is referred to by another package.
This may mean that the package is missing, has been obsoleted, or
is only available from another source

E: Package 'docker-ce' has no installation candidate
E: Unable to locate package docker-ce-cli
shih@DESKTOP-EVK789N:~$ docker --v

Command 'docker' not found, but can be installed with:

sudo apt install docker.io

shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce-cli
[sudo] password for shih:
Reading package lists... Done
Building dependency tree
Reading state information... Done
E: Unable to locate package docker-ce-cli
shih@DESKTOP-EVK789N:~$ docker

Command 'docker' not found, but can be installed with:

sudo apt install docker.io

shih@DESKTOP-EVK789N:~$ sudo apt-get update
Hit:1 http://security.ubuntu.com/ubuntu focal-security InRelease
Hit:2 http://archive.ubuntu.com/ubuntu focal InRelease
Hit:3 http://archive.ubuntu.com/ubuntu focal-updates InRelease
Hit:4 http://archive.ubuntu.com/ubuntu focal-backports InRelease
Reading package lists... Done
shih@DESKTOP-EVK789N:~$ sudo apt-cache madison docker-ce
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce docker-ce-cli containerd.io
Reading package lists... Done
Building dependency tree
Reading state information... Done
Package docker-ce is not available, but is referred to by another package.
This may mean that the package is missing, has been obsoleted, or
is only available from another source

E: Package 'docker-ce' has no installation candidate
E: Unable to locate package docker-ce-cli
E: Unable to locate package containerd.io
E: Couldn't find any package by glob 'containerd.io'
E: Couldn't find any package by regex 'containerd.io'
shih@DESKTOP-EVK789N:~$ sudo docker run hello-world
sudo: docker: command not found
shih@DESKTOP-EVK789N:~$ sudo apt-get install \
>     ca-certificates \
>     curl \
>     gnupg \
>     lsb-release
Reading package lists... Done
Building dependency tree
Reading state information... Done
lsb-release is already the newest version (11.1.0ubuntu2).
lsb-release set to manually installed.
The following additional packages will be installed:
  dirmngr gnupg-l10n gnupg-utils gpg gpg-agent gpg-wks-client gpg-wks-server gpgconf gpgsm gpgv libcurl4
Suggested packages:
  pinentry-gnome3 tor parcimonie xloadimage scdaemon
The following packages will be upgraded:
  ca-certificates curl dirmngr gnupg gnupg-l10n gnupg-utils gpg gpg-agent gpg-wks-client gpg-wks-server gpgconf gpgsm
  gpgv libcurl4
14 upgraded, 0 newly installed, 0 to remove and 237 not upgraded.
Need to get 3104 kB of archives.
After this operation, 2048 B disk space will be freed.
Do you want to continue? [Y/n] Y
Get:1 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gpg-wks-client amd64 2.2.19-3ubuntu2.1 [97.6 kB]
Get:2 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 dirmngr amd64 2.2.19-3ubuntu2.1 [329 kB]
Get:3 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gnupg-utils amd64 2.2.19-3ubuntu2.1 [480 kB]
Get:4 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gpg-wks-server amd64 2.2.19-3ubuntu2.1 [90.3 kB]
Get:5 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gpg-agent amd64 2.2.19-3ubuntu2.1 [232 kB]
Get:6 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gpg amd64 2.2.19-3ubuntu2.1 [483 kB]
Get:7 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gpgconf amd64 2.2.19-3ubuntu2.1 [124 kB]
Get:8 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gnupg-l10n all 2.2.19-3ubuntu2.1 [51.7 kB]
Get:9 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gnupg all 2.2.19-3ubuntu2.1 [259 kB]
Get:10 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gpgsm amd64 2.2.19-3ubuntu2.1 [217 kB]
Get:11 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 gpgv amd64 2.2.19-3ubuntu2.1 [199 kB]
Get:12 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 ca-certificates all 20210119~20.04.2 [145 kB]
Get:13 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 curl amd64 7.68.0-1ubuntu2.7 [161 kB]
Get:14 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 libcurl4 amd64 7.68.0-1ubuntu2.7 [234 kB]
Fetched 3104 kB in 4s (791 kB/s)
Preconfiguring packages ...
(Reading database ... 31836 files and directories currently installed.)
Preparing to unpack .../00-gpg-wks-client_2.2.19-3ubuntu2.1_amd64.deb ...
Unpacking gpg-wks-client (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../01-dirmngr_2.2.19-3ubuntu2.1_amd64.deb ...
Unpacking dirmngr (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../02-gnupg-utils_2.2.19-3ubuntu2.1_amd64.deb ...
Unpacking gnupg-utils (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../03-gpg-wks-server_2.2.19-3ubuntu2.1_amd64.deb ...
Unpacking gpg-wks-server (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../04-gpg-agent_2.2.19-3ubuntu2.1_amd64.deb ...
Unpacking gpg-agent (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../05-gpg_2.2.19-3ubuntu2.1_amd64.deb ...
Unpacking gpg (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../06-gpgconf_2.2.19-3ubuntu2.1_amd64.deb ...
Unpacking gpgconf (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../07-gnupg-l10n_2.2.19-3ubuntu2.1_all.deb ...
Unpacking gnupg-l10n (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../08-gnupg_2.2.19-3ubuntu2.1_all.deb ...
Unpacking gnupg (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../09-gpgsm_2.2.19-3ubuntu2.1_amd64.deb ...
Unpacking gpgsm (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Preparing to unpack .../10-gpgv_2.2.19-3ubuntu2.1_amd64.deb ...
Unpacking gpgv (2.2.19-3ubuntu2.1) over (2.2.19-3ubuntu2) ...
Setting up gpgv (2.2.19-3ubuntu2.1) ...
(Reading database ... 31836 files and directories currently installed.)
Preparing to unpack .../ca-certificates_20210119~20.04.2_all.deb ...
Unpacking ca-certificates (20210119~20.04.2) over (20190110ubuntu1) ...
Preparing to unpack .../curl_7.68.0-1ubuntu2.7_amd64.deb ...
Unpacking curl (7.68.0-1ubuntu2.7) over (7.68.0-1ubuntu2) ...
Preparing to unpack .../libcurl4_7.68.0-1ubuntu2.7_amd64.deb ...
Unpacking libcurl4:amd64 (7.68.0-1ubuntu2.7) over (7.68.0-1ubuntu2) ...
Setting up ca-certificates (20210119~20.04.2) ...
Updating certificates in /etc/ssl/certs...
21 added, 21 removed; done.
Setting up gnupg-l10n (2.2.19-3ubuntu2.1) ...
Setting up gpgconf (2.2.19-3ubuntu2.1) ...
Setting up libcurl4:amd64 (7.68.0-1ubuntu2.7) ...
Setting up curl (7.68.0-1ubuntu2.7) ...
Setting up gpg (2.2.19-3ubuntu2.1) ...
Setting up gnupg-utils (2.2.19-3ubuntu2.1) ...
Setting up gpg-agent (2.2.19-3ubuntu2.1) ...
Setting up gpgsm (2.2.19-3ubuntu2.1) ...
Setting up dirmngr (2.2.19-3ubuntu2.1) ...
Setting up gpg-wks-server (2.2.19-3ubuntu2.1) ...
Setting up gpg-wks-client (2.2.19-3ubuntu2.1) ...
Setting up gnupg (2.2.19-3ubuntu2.1) ...
Processing triggers for libc-bin (2.31-0ubuntu9) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for install-info (6.7.0.dfsg.2-5) ...
Processing triggers for ca-certificates (20210119~20.04.2) ...
Updating certificates in /etc/ssl/certs...
0 added, 0 removed; done.
Running hooks in /etc/ca-certificates/update.d...
done.
shih@DESKTOP-EVK789N:~$ sudo docker run hello-world
sudo: docker: command not found
shih@DESKTOP-EVK789N:~$ sudo docker
sudo: docker: command not found
shih@DESKTOP-EVK789N:~$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
shih@DESKTOP-EVK789N:~$ echo \
>   "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
lsb_re>   $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
shih@DESKTOP-EVK789N:~$ sudo apt-get update
Get:1 https://download.docker.com/linux/ubuntu focal InRelease [57.7 kB]
Get:2 https://download.docker.com/linux/ubuntu focal/stable amd64 Packages [13.5 kB]
Hit:3 http://archive.ubuntu.com/ubuntu focal InRelease
Hit:4 http://security.ubuntu.com/ubuntu focal-security InRelease
Hit:5 http://archive.ubuntu.com/ubuntu focal-updates InRelease
Get:6 http://archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]
Fetched 180 kB in 3s (66.3 kB/s)
Reading package lists... Done
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce docker-ce-cli containerd.io
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following additional packages will be installed:
  docker-ce-rootless-extras docker-scan-plugin pigz slirp4netns
Suggested packages:
  aufs-tools cgroupfs-mount | cgroup-lite
The following NEW packages will be installed:
  containerd.io docker-ce docker-ce-cli docker-ce-rootless-extras docker-scan-plugin pigz slirp4netns
0 upgraded, 7 newly installed, 0 to remove and 237 not upgraded.
Need to get 97.2 MB of archives.
After this operation, 409 MB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 https://download.docker.com/linux/ubuntu focal/stable amd64 containerd.io amd64 1.4.12-1 [23.7 MB]
Get:2 http://archive.ubuntu.com/ubuntu focal/universe amd64 pigz amd64 2.4-1 [57.4 kB]
Get:3 http://archive.ubuntu.com/ubuntu focal/universe amd64 slirp4netns amd64 0.4.3-1 [74.3 kB]
Get:4 https://download.docker.com/linux/ubuntu focal/stable amd64 docker-ce-cli amd64 5:20.10.12~3-0~ubuntu-focal [40.7 MB]
Get:5 https://download.docker.com/linux/ubuntu focal/stable amd64 docker-ce amd64 5:20.10.12~3-0~ubuntu-focal [21.2 MB]
Get:6 https://download.docker.com/linux/ubuntu focal/stable amd64 docker-ce-rootless-extras amd64 5:20.10.12~3-0~ubuntu-focal [7921 kB]
Get:7 https://download.docker.com/linux/ubuntu focal/stable amd64 docker-scan-plugin amd64 0.12.0~ubuntu-focal [3518 kB]
Fetched 97.2 MB in 12s (7843 kB/s)
Selecting previously unselected package pigz.
(Reading database ... 31836 files and directories currently installed.)
Preparing to unpack .../0-pigz_2.4-1_amd64.deb ...
Unpacking pigz (2.4-1) ...
Selecting previously unselected package containerd.io.
Preparing to unpack .../1-containerd.io_1.4.12-1_amd64.deb ...
Unpacking containerd.io (1.4.12-1) ...
Selecting previously unselected package docker-ce-cli.
Preparing to unpack .../2-docker-ce-cli_5%3a20.10.12~3-0~ubuntu-focal_amd64.deb ...
Unpacking docker-ce-cli (5:20.10.12~3-0~ubuntu-focal) ...
Selecting previously unselected package docker-ce.
Preparing to unpack .../3-docker-ce_5%3a20.10.12~3-0~ubuntu-focal_amd64.deb ...
Unpacking docker-ce (5:20.10.12~3-0~ubuntu-focal) ...
Selecting previously unselected package docker-ce-rootless-extras.
Preparing to unpack .../4-docker-ce-rootless-extras_5%3a20.10.12~3-0~ubuntu-focal_amd64.deb ...
Unpacking docker-ce-rootless-extras (5:20.10.12~3-0~ubuntu-focal) ...
Selecting previously unselected package docker-scan-plugin.
Preparing to unpack .../5-docker-scan-plugin_0.12.0~ubuntu-focal_amd64.deb ...
Unpacking docker-scan-plugin (0.12.0~ubuntu-focal) ...
Selecting previously unselected package slirp4netns.
Preparing to unpack .../6-slirp4netns_0.4.3-1_amd64.deb ...
Unpacking slirp4netns (0.4.3-1) ...
Setting up slirp4netns (0.4.3-1) ...
Setting up docker-scan-plugin (0.12.0~ubuntu-focal) ...
Setting up containerd.io (1.4.12-1) ...
Created symlink /etc/systemd/system/multi-user.target.wants/containerd.service → /lib/systemd/system/containerd.service.
Setting up docker-ce-cli (5:20.10.12~3-0~ubuntu-focal) ...
Setting up pigz (2.4-1) ...
Setting up docker-ce-rootless-extras (5:20.10.12~3-0~ubuntu-focal) ...
Setting up docker-ce (5:20.10.12~3-0~ubuntu-focal) ...
Created symlink /etc/systemd/system/multi-user.target.wants/docker.service → /lib/systemd/system/docker.service.
Created symlink /etc/systemd/system/sockets.target.wants/docker.socket → /lib/systemd/system/docker.socket.
invoke-rc.d: could not determine current runlevel
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for systemd (245.4-4ubuntu3) ...
shih@DESKTOP-EVK789N:~$ sudo apt-cache madison docker-ce
 docker-ce | 5:20.10.12~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.11~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.10~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.9~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.8~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.7~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.6~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.5~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.4~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.3~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.2~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.1~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:20.10.0~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:19.03.15~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:19.03.14~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:19.03.13~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:19.03.12~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:19.03.11~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:19.03.10~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
 docker-ce | 5:19.03.9~3-0~ubuntu-focal | https://download.docker.com/linux/ubuntu focal/stable amd64 Packages
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce=<VERSION_STRING> docker-ce-cli=<VERSION_STRING> containerd.io
-bash: VERSION_STRING: No such file or directory
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce=5:18.09.9~3–0~ubuntu-bionic docker-ce-cli=5:18.09.9~3–0~ubuntu-bionic containerd.io
Reading package lists... Done
Building dependency tree
Reading state information... Done
E: Version '5:18.09.9~3–0~ubuntu-bionic' for 'docker-ce' was not found
E: Version '5:18.09.9~3–0~ubuntu-bionic' for 'docker-ce-cli' was not found
shih@DESKTOP-EVK789N:~$ docker — version
docker: '—' is not a docker command.
See 'docker --help'
shih@DESKTOP-EVK789N:~$ docker --version
docker--version: command not found
shih@DESKTOP-EVK789N:~$ docker --version
Docker version 20.10.12, build e91ed57
shih@DESKTOP-EVK789N:~$ sudo service docker status
 * Docker is not running
shih@DESKTOP-EVK789N:~$ sudo docker -v
Docker version 20.10.12, build e91ed57
shih@DESKTOP-EVK789N:~$ docker version
Client: Docker Engine - Community
 Version:           20.10.12
 API version:       1.41
 Go version:        go1.16.12
 Git commit:        e91ed57
 Built:             Mon Dec 13 11:45:33 2021
 OS/Arch:           linux/amd64
 Context:           default
 Experimental:      true
Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?
shih@DESKTOP-EVK789N:~$ sudo docker run hello-world
docker: Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?.
See 'docker run --help'.
shih@DESKTOP-EVK789N:~$ sudo docker run
"docker run" requires at least 1 argument.
See 'docker run --help'.

Usage:  docker run [OPTIONS] IMAGE [COMMAND] [ARG...]

Run a command in a new container
shih@DESKTOP-EVK789N:~$ docker images
Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?
shih@DESKTOP-EVK789N:~$ sudo docker images
Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?
shih@DESKTOP-EVK789N:~$ sudo docker pull alpine:latest
Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?
shih@DESKTOP-EVK789N:~$ ls
shih@DESKTOP-EVK789N:~$ docker container ls
Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?
shih@DESKTOP-EVK789N:~$ docker run hello-world
docker: Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?.
See 'docker run --help'.
shih@DESKTOP-EVK789N:~$ sudo service docker status
 * Docker is not running
shih@DESKTOP-EVK789N:~$ sudo service docker restart
shih@DESKTOP-EVK789N:~$ sudo service docker status
 * Docker is not running
shih@DESKTOP-EVK789N:~$ sudo docker run hello-world
docker: Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?.
See 'docker run --help'.
shih@DESKTOP-EVK789N:~$ sudo docker run --help

Usage:  docker run [OPTIONS] IMAGE [COMMAND] [ARG...]

Run a command in a new container

Options:
      --add-host list                  Add a custom host-to-IP mapping (host:ip)
  -a, --attach list                    Attach to STDIN, STDOUT or STDERR
      --blkio-weight uint16            Block IO (relative weight), between 10 and 1000, or 0 to disable (default 0)
      --blkio-weight-device list       Block IO weight (relative device weight) (default [])
      --cap-add list                   Add Linux capabilities
      --cap-drop list                  Drop Linux capabilities
      --cgroup-parent string           Optional parent cgroup for the container
      --cgroupns string                Cgroup namespace to use (host|private)
                                       'host':    Run the container in the Docker host's cgroup namespace
                                       'private': Run the container in its own private cgroup namespace
                                       '':        Use the cgroup namespace as configured by the
                                                  default-cgroupns-mode option on the daemon (default)
      --cidfile string                 Write the container ID to the file
      --cpu-period int                 Limit CPU CFS (Completely Fair Scheduler) period
      --cpu-quota int                  Limit CPU CFS (Completely Fair Scheduler) quota
      --cpu-rt-period int              Limit CPU real-time period in microseconds
      --cpu-rt-runtime int             Limit CPU real-time runtime in microseconds
  -c, --cpu-shares int                 CPU shares (relative weight)
      --cpus decimal                   Number of CPUs
      --cpuset-cpus string             CPUs in which to allow execution (0-3, 0,1)
      --cpuset-mems string             MEMs in which to allow execution (0-3, 0,1)
  -d, --detach                         Run container in background and print container ID
      --detach-keys string             Override the key sequence for detaching a container
      --device list                    Add a host device to the container
      --device-cgroup-rule list        Add a rule to the cgroup allowed devices list
      --device-read-bps list           Limit read rate (bytes per second) from a device (default [])
      --device-read-iops list          Limit read rate (IO per second) from a device (default [])
      --device-write-bps list          Limit write rate (bytes per second) to a device (default [])
      --device-write-iops list         Limit write rate (IO per second) to a device (default [])
      --disable-content-trust          Skip image verification (default true)
      --dns list                       Set custom DNS servers
      --dns-option list                Set DNS options
      --dns-search list                Set custom DNS search domains
      --domainname string              Container NIS domain name
      --entrypoint string              Overwrite the default ENTRYPOINT of the image
  -e, --env list                       Set environment variables
      --env-file list                  Read in a file of environment variables
      --expose list                    Expose a port or a range of ports
      --gpus gpu-request               GPU devices to add to the container ('all' to pass all GPUs)
      --group-add list                 Add additional groups to join
      --health-cmd string              Command to run to check health
      --health-interval duration       Time between running the check (ms|s|m|h) (default 0s)
      --health-retries int             Consecutive failures needed to report unhealthy
      --health-start-period duration   Start period for the container to initialize before starting
                                       health-retries countdown (ms|s|m|h) (default 0s)
      --health-timeout duration        Maximum time to allow one check to run (ms|s|m|h) (default 0s)
      --help                           Print usage
  -h, --hostname string                Container host name
      --init                           Run an init inside the container that forwards signals and reaps processes
  -i, --interactive                    Keep STDIN open even if not attached
      --ip string                      IPv4 address (e.g., 172.30.100.104)
      --ip6 string                     IPv6 address (e.g., 2001:db8::33)
      --ipc string                     IPC mode to use
      --isolation string               Container isolation technology
      --kernel-memory bytes            Kernel memory limit
  -l, --label list                     Set meta data on a container
      --label-file list                Read in a line delimited file of labels
      --link list                      Add link to another container
      --link-local-ip list             Container IPv4/IPv6 link-local addresses
      --log-driver string              Logging driver for the container
      --log-opt list                   Log driver options
      --mac-address string             Container MAC address (e.g., 92:d0:c6:0a:29:33)
  -m, --memory bytes                   Memory limit
      --memory-reservation bytes       Memory soft limit
      --memory-swap bytes              Swap limit equal to memory plus swap: '-1' to enable unlimited swap
      --memory-swappiness int          Tune container memory swappiness (0 to 100) (default -1)
      --mount mount                    Attach a filesystem mount to the container
      --name string                    Assign a name to the container
      --network network                Connect a container to a network
      --network-alias list             Add network-scoped alias for the container
      --no-healthcheck                 Disable any container-specified HEALTHCHECK
      --oom-kill-disable               Disable OOM Killer
      --oom-score-adj int              Tune host's OOM preferences (-1000 to 1000)
      --pid string                     PID namespace to use
      --pids-limit int                 Tune container pids limit (set -1 for unlimited)
      --platform string                Set platform if server is multi-platform capable
      --privileged                     Give extended privileges to this container
  -p, --publish list                   Publish a container's port(s) to the host
  -P, --publish-all                    Publish all exposed ports to random ports
      --pull string                    Pull image before running ("always"|"missing"|"never") (default "missing")
      --read-only                      Mount the container's root filesystem as read only
      --restart string                 Restart policy to apply when a container exits (default "no")
      --rm                             Automatically remove the container when it exits
      --runtime string                 Runtime to use for this container
      --security-opt list              Security Options
      --shm-size bytes                 Size of /dev/shm
      --sig-proxy                      Proxy received signals to the process (default true)
      --stop-signal string             Signal to stop a container (default "SIGTERM")
      --stop-timeout int               Timeout (in seconds) to stop a container
      --storage-opt list               Storage driver options for the container
      --sysctl map                     Sysctl options (default map[])
      --tmpfs list                     Mount a tmpfs directory
  -t, --tty                            Allocate a pseudo-TTY
      --ulimit ulimit                  Ulimit options (default [])
  -u, --user string                    Username or UID (format: <name|uid>[:<group|gid>])
      --userns string                  User namespace to use
      --uts string                     UTS namespace to use
  -v, --volume list                    Bind mount a volume
      --volume-driver string           Optional volume driver for the container
      --volumes-from list              Mount volumes from the specified container(s)
  -w, --workdir string                 Working directory inside the container
shih@DESKTOP-EVK789N:~$ sudo docker -d run --help
unknown shorthand flag: 'd' in -d
See 'docker --help'.

Usage:  docker [OPTIONS] COMMAND

A self-sufficient runtime for containers

Options:
      --config string      Location of client config files (default "/root/.docker")
  -c, --context string     Name of the context to use to connect to the daemon (overrides DOCKER_HOST env var and
                           default context set with "docker context use")
  -D, --debug              Enable debug mode
  -H, --host list          Daemon socket(s) to connect to
  -l, --log-level string   Set the logging level ("debug"|"info"|"warn"|"error"|"fatal") (default "info")
      --tls                Use TLS; implied by --tlsverify
      --tlscacert string   Trust certs signed only by this CA (default "/root/.docker/ca.pem")
      --tlscert string     Path to TLS certificate file (default "/root/.docker/cert.pem")
      --tlskey string      Path to TLS key file (default "/root/.docker/key.pem")
      --tlsverify          Use TLS and verify the remote
  -v, --version            Print version information and quit

Management Commands:
  app*        Docker App (Docker Inc., v0.9.1-beta3)
  builder     Manage builds
  buildx*     Docker Buildx (Docker Inc., v0.7.1-docker)
  config      Manage Docker configs
  container   Manage containers
  context     Manage contexts
  image       Manage images
  manifest    Manage Docker image manifests and manifest lists
  network     Manage networks
  node        Manage Swarm nodes
  plugin      Manage plugins
  scan*       Docker Scan (Docker Inc., v0.12.0)
  secret      Manage Docker secrets
  service     Manage services
  stack       Manage Docker stacks
  swarm       Manage Swarm
  system      Manage Docker
  trust       Manage trust on Docker images
  volume      Manage volumes

Commands:
  attach      Attach local standard input, output, and error streams to a running container
  build       Build an image from a Dockerfile
  commit      Create a new image from a container's changes
  cp          Copy files/folders between a container and the local filesystem
  create      Create a new container
  diff        Inspect changes to files or directories on a container's filesystem
  events      Get real time events from the server
  exec        Run a command in a running container
  export      Export a container's filesystem as a tar archive
  history     Show the history of an image
  images      List images
  import      Import the contents from a tarball to create a filesystem image
  info        Display system-wide information
  inspect     Return low-level information on Docker objects
  kill        Kill one or more running containers
  load        Load an image from a tar archive or STDIN
  login       Log in to a Docker registry
  logout      Log out from a Docker registry
  logs        Fetch the logs of a container
  pause       Pause all processes within one or more containers
  port        List port mappings or a specific mapping for the container
  ps          List containers
  pull        Pull an image or a repository from a registry
  push        Push an image or a repository to a registry
  rename      Rename a container
  restart     Restart one or more containers
  rm          Remove one or more containers
  rmi         Remove one or more images
  run         Run a command in a new container
  save        Save one or more images to a tar archive (streamed to STDOUT by default)
  search      Search the Docker Hub for images
  start       Start one or more stopped containers
  stats       Display a live stream of container(s) resource usage statistics
  stop        Stop one or more running containers
  tag         Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
  top         Display the running processes of a container
  unpause     Unpause all processes within one or more containers
  update      Update configuration of one or more containers
  version     Show the Docker version information
  wait        Block until one or more containers stop, then print their exit codes

Run 'docker COMMAND --help' for more information on a command.

To get more help with docker, check out our guides at https://docs.docker.com/go/guides/

shih@DESKTOP-EVK789N:~$ sudo docker -d -it run --help
unknown shorthand flag: 'd' in -d
See 'docker --help'.

Usage:  docker [OPTIONS] COMMAND

A self-sufficient runtime for containers

Options:
      --config string      Location of client config files (default "/root/.docker")
  -c, --context string     Name of the context to use to connect to the daemon (overrides DOCKER_HOST env var and
                           default context set with "docker context use")
  -D, --debug              Enable debug mode
  -H, --host list          Daemon socket(s) to connect to
  -l, --log-level string   Set the logging level ("debug"|"info"|"warn"|"error"|"fatal") (default "info")
      --tls                Use TLS; implied by --tlsverify
      --tlscacert string   Trust certs signed only by this CA (default "/root/.docker/ca.pem")
      --tlscert string     Path to TLS certificate file (default "/root/.docker/cert.pem")
      --tlskey string      Path to TLS key file (default "/root/.docker/key.pem")
      --tlsverify          Use TLS and verify the remote
  -v, --version            Print version information and quit

Management Commands:
  app*        Docker App (Docker Inc., v0.9.1-beta3)
  builder     Manage builds
  buildx*     Docker Buildx (Docker Inc., v0.7.1-docker)
  config      Manage Docker configs
  container   Manage containers
  context     Manage contexts
  image       Manage images
  manifest    Manage Docker image manifests and manifest lists
  network     Manage networks
  node        Manage Swarm nodes
  plugin      Manage plugins
  scan*       Docker Scan (Docker Inc., v0.12.0)
  secret      Manage Docker secrets
  service     Manage services
  stack       Manage Docker stacks
  swarm       Manage Swarm
  system      Manage Docker
  trust       Manage trust on Docker images
  volume      Manage volumes

Commands:
  attach      Attach local standard input, output, and error streams to a running container
  build       Build an image from a Dockerfile
  commit      Create a new image from a container's changes
  cp          Copy files/folders between a container and the local filesystem
  create      Create a new container
  diff        Inspect changes to files or directories on a container's filesystem
  events      Get real time events from the server
  exec        Run a command in a running container
  export      Export a container's filesystem as a tar archive
  history     Show the history of an image
  images      List images
  import      Import the contents from a tarball to create a filesystem image
  info        Display system-wide information
  inspect     Return low-level information on Docker objects
  kill        Kill one or more running containers
  load        Load an image from a tar archive or STDIN
  login       Log in to a Docker registry
  logout      Log out from a Docker registry
  logs        Fetch the logs of a container
  pause       Pause all processes within one or more containers
  port        List port mappings or a specific mapping for the container
  ps          List containers
  pull        Pull an image or a repository from a registry
  push        Push an image or a repository to a registry
  rename      Rename a container
  restart     Restart one or more containers
  rm          Remove one or more containers
  rmi         Remove one or more images
  run         Run a command in a new container
  save        Save one or more images to a tar archive (streamed to STDOUT by default)
  search      Search the Docker Hub for images
  start       Start one or more stopped containers
  stats       Display a live stream of container(s) resource usage statistics
  stop        Stop one or more running containers
  tag         Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
  top         Display the running processes of a container
  unpause     Unpause all processes within one or more containers
  update      Update configuration of one or more containers
  version     Show the Docker version information
  wait        Block until one or more containers stop, then print their exit codes

Run 'docker COMMAND --help' for more information on a command.

To get more help with docker, check out our guides at https://docs.docker.com/go/guides/

shih@DESKTOP-EVK789N:~$ service docker start
 * Docker must be run as root
shih@DESKTOP-EVK789N:~$
```

---



# WSL



---
## How to Install Windows Subsystem for Linux in Windows 11
https://www.tomshardware.com/how-to/get-started-windows-subsystem-for-linux-windows-11
### wsl 為內建指令
1. PowerShell or Command Prompt “Run as administrator”
2. Enter the following command: 
    $ wsl --install
3. Restart your PC. WSL will install itself after your reboot. 重新啟動您的電腦。應該會出現一條通知，告訴您 WSL 已安裝，並且在您重新啟動 PC 後可以使用。 
4. 開機後 會自動執行 ubuntu 並要設定帳號與密碼 Enter a username and password when prompted by WSL. 
5. 安裝不同的 Linux 發行版 
    $ wsl --list --online
    $ wsl --install -d <Distro>
    
        Ex: wsl --install -d Debian
        Ex: wsl --install -d Kali-Linux 
6. Microsoft Store 安裝 Linux  微軟商店 
7. 搜索 “Linux” 單擊您感興趣的發行版，然後單擊“安裝”
8. 更新 WSL：
    $ wsl --update
9. 重新啟動wsl
    $ wsl --shutdown

---
```
Microsoft Windows [版本 10.0.22000.376]
(c) Microsoft Corporation. 著作權所有，並保留一切權利。

C:\Users\LC55-14C>wsl

Copyright (c) Microsoft Corporation. 著作權所有，並保留一切權利。

使用方式: wsl.exe [引數]

引數:

    --install <Options>
        安裝 Windows 子系統 Linux 版功能。如果未指定任何選項，
        建議的功能將與預設發佈一起安裝。

        若要檢視預設發佈及其他有效發佈的清單，
        請使用 'wsl --list --online'。

        選項:
            --distribution, -d [Argument]
                依名稱指定要下載及安裝的發佈。

            參數:
                有效的發佈名稱 (不區分大小寫)。

            範例:
                wsl --install -d Ubuntu
                wsl --install --distribution Debian

    --list, -l [Options]
        列出發佈。

        選項:
            --online, -o
                使用 'wsl --install' 顯示可安裝的可用發佈。

    --狀態
        顯示 Windows 子系統 Linux 版狀態。

    --說明
            顯示使用狀況資訊。

C:\Users\LC55-14C>
```
---

---
```
Windows PowerShell
著作權（C） Microsoft Corporation。保留擁有權利。

安裝最新的 PowerShell 以取得新功能和改進功能！https://aka.ms/PSWindows

PS C:\Windows\system32> wsl --install
正在安裝：Windows 子系統 Linux 版
已完成安裝 Windows 子系統 Linux 版。
正在下載：WSL Kernel
正在安裝：WSL Kernel
已完成安裝 WSL Kernel。
正在下載：GUI [應用程式支援]
正在安裝：GUI [應用程式支援]
已完成安裝 GUI [應用程式支援]。
正在下載：Ubuntu
已成功執行所要求的操作。請重新開機，變更才能生效。
PS C:\Windows\system32>
```

---
## 帳號 : shih (第一碼不可大寫)
## 密碼 : 1 (密碼長度不限 輸入時不顯示)
```

Installing, this may take a few minutes...
Please create a default UNIX user account. The username does not need to match your Windows username.
For more information visit: https://aka.ms/wslusers
Enter new UNIX username: Shih
adduser: Please enter a username matching the regular expression configured
via the NAME_REGEX[_SYSTEM] configuration variable.  Use the `--force-badname'
option to relax this check or reconfigure NAME_REGEX.
Enter new UNIX username: shih
New password:
Retype new password:
passwd: password updated successfully
Installation successful!
To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

Welcome to Ubuntu 20.04 LTS (GNU/Linux 5.10.16.3-microsoft-standard-WSL2 x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Wed Jan 12 15:38:45 CST 2022

  System load:  0.0                Processes:             8
  Usage of /:   0.4% of 250.98GB   Users logged in:       0
  Memory usage: 7%                 IPv4 address for eth0: 172.20.25.96
  Swap usage:   0%

0 updates can be installed immediately.
0 of these updates are security updates.


The list of available updates is more than a week old.
To check for new updates run: sudo apt update


This message is shown once once a day. To disable it please create the
/home/shih/.hushlogin file.
shih@DESKTOP-EVK789N:~$
```
---
## 安裝第二個 linux (裝好會立即啟動不用重開機)

```
Windows PowerShell
著作權（C） Microsoft Corporation。保留擁有權利。

安裝最新的 PowerShell 以取得新功能和改進功能！https://aka.ms/PSWindows

PS C:\Windows\system32> wsl --list
Windows 子系統 Linux 版發佈:
Ubuntu (預設值)
PS C:\Windows\system32> wsl --list --online
以下是可安裝之有效發佈的清單。
使用 'wsl --install -d <Distro>' 安裝。

NAME            FRIENDLY NAME
Ubuntu          Ubuntu
Debian          Debian GNU/Linux
kali-linux      Kali Linux Rolling
openSUSE-42     openSUSE Leap 42
SLES-12         SUSE Linux Enterprise Server v12
Ubuntu-16.04    Ubuntu 16.04 LTS
Ubuntu-18.04    Ubuntu 18.04 LTS
Ubuntu-20.04    Ubuntu 20.04 LTS
PS C:\Windows\system32> wsl --install -d Kali-Linux
正在下載：Kali Linux Rolling
正在安裝：Kali Linux Rolling
已完成安裝 Kali Linux Rolling。
正在啟動 Kali Linux Rolling...
PS C:\Windows\system32>
```
---
```
PS C:\Windows\system32> wsl --list --online
以下是可安裝的有效通訊群組清單。
「*」表示預設的通訊群組。
使用「wsl--安裝-d 」安裝。<Distro>

  NAME            FRIENDLY NAME
* Ubuntu          Ubuntu
  Debian          Debian GNU/Linux
  kali-linux      Kali Linux Rolling
  openSUSE-42     openSUSE Leap 42
  SLES-12         SUSE Linux Enterprise Server v12
  Ubuntu-16.04    Ubuntu 16.04 LTS
  Ubuntu-18.04    Ubuntu 18.04 LTS
  Ubuntu-20.04    Ubuntu 20.04 LTS
PS C:\Windows\system32>
```

---
```
shih@DESKTOP-EVK789N:~$ sudo apt-get update
Hit:1 https://download.docker.com/linux/ubuntu focal InRelease
Hit:2 http://archive.ubuntu.com/ubuntu focal InRelease
Get:3 http://security.ubuntu.com/ubuntu focal-security InRelease [114 kB]
Get:4 http://archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]
Get:5 http://archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]
Fetched 336 kB in 3s (119 kB/s)
Reading package lists... Done
shih@DESKTOP-EVK789N:~$ sudo apt-get install \
>     apt-transport-https \
>     ca-certificates \
>     curl \
>     gnupg-agent \
>     software-properties-common
Reading package lists... Done
Building dependency tree
Reading state information... Done
ca-certificates is already the newest version (20210119~20.04.2).
ca-certificates set to manually installed.
curl is already the newest version (7.68.0-1ubuntu2.7).
The following additional packages will be installed:
  python3-software-properties
The following NEW packages will be installed:
  apt-transport-https gnupg-agent
The following packages will be upgraded:
  python3-software-properties software-properties-common
2 upgraded, 2 newly installed, 0 to remove and 235 not upgraded.
Need to get 45.4 kB of archives.
After this operation, 208 kB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://archive.ubuntu.com/ubuntu focal-updates/universe amd64 apt-transport-https all 2.0.6 [4680 B]
Get:2 http://archive.ubuntu.com/ubuntu focal-updates/universe amd64 gnupg-agent all 2.2.19-3ubuntu2.1 [5232 B]
Get:3 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 software-properties-common all 0.99.9.8 [10.6 kB]
Get:4 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 python3-software-properties all 0.99.9.8 [24.9 kB]
Fetched 45.4 kB in 1s (34.6 kB/s)
Selecting previously unselected package apt-transport-https.
(Reading database ... 32087 files and directories currently installed.)
Preparing to unpack .../apt-transport-https_2.0.6_all.deb ...
Unpacking apt-transport-https (2.0.6) ...
Selecting previously unselected package gnupg-agent.
Preparing to unpack .../gnupg-agent_2.2.19-3ubuntu2.1_all.deb ...
Unpacking gnupg-agent (2.2.19-3ubuntu2.1) ...
Preparing to unpack .../software-properties-common_0.99.9.8_all.deb ...
Unpacking software-properties-common (0.99.9.8) over (0.98.9) ...
Preparing to unpack .../python3-software-properties_0.99.9.8_all.deb ...
Unpacking python3-software-properties (0.99.9.8) over (0.98.9) ...
Setting up apt-transport-https (2.0.6) ...
Setting up python3-software-properties (0.99.9.8) ...
Setting up gnupg-agent (2.2.19-3ubuntu2.1) ...
Setting up software-properties-common (0.99.9.8) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for dbus (1.12.16-2ubuntu2) ...
shih@DESKTOP-EVK789N:~$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
OK
shih@DESKTOP-EVK789N:~$ sudo add-apt-repository \
>    "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
>    $(lsb_release -cs) \
>    stable"
Hit:1 https://download.docker.com/linux/ubuntu focal InRelease
Hit:2 http://archive.ubuntu.com/ubuntu focal InRelease
Get:3 http://security.ubuntu.com/ubuntu focal-security InRelease [114 kB]
Get:4 http://archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]
Get:5 http://archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]
Fetched 336 kB in 2s (139 kB/s)
Reading package lists... Done
W: Target Packages (stable/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Translations (stable/i18n/Translation-en) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-amd64) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-all) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Translations (stable/i18n/Translation-en) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-amd64) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-all) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
shih@DESKTOP-EVK789N:~$ sudo apt-get update
Hit:1 https://download.docker.com/linux/ubuntu focal InRelease
Get:2 http://security.ubuntu.com/ubuntu focal-security InRelease [114 kB]
Hit:3 http://archive.ubuntu.com/ubuntu focal InRelease
Get:4 http://archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]
Get:5 http://archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]
Fetched 336 kB in 2s (147 kB/s)
Reading package lists... Done
W: Target Packages (stable/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Translations (stable/i18n/Translation-en) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-amd64) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-all) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Translations (stable/i18n/Translation-en) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-amd64) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-all) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce docker-ce-cli containerd.io
Reading package lists... Done
Building dependency tree
Reading state information... Done
containerd.io is already the newest version (1.4.12-1).
docker-ce-cli is already the newest version (5:20.10.12~3-0~ubuntu-focal).
docker-ce is already the newest version (5:20.10.12~3-0~ubuntu-focal).
0 upgraded, 0 newly installed, 0 to remove and 235 not upgraded.
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce=<VERSION_STRING> docker-ce-cli=<VERSION_STRING> containe
-bash: VERSION_STRING: No such file or directory
shih@DESKTOP-EVK789N:~$ sudo docker -v
Docker version 20.10.12, build e91ed57
shih@DESKTOP-EVK789N:~$ sudo service docker status
 * Docker is not running
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce=5:18.09.9~3–0~ubuntu-bionic docker-ce-cli=5:18.09.9~3–0~ubuntu-bionic containerd.io
Reading package lists... Done
Building dependency tree
Reading state information... Done
E: Version '5:18.09.9~3–0~ubuntu-bionic' for 'docker-ce' was not found
E: Version '5:18.09.9~3–0~ubuntu-bionic' for 'docker-ce-cli' was not found
shih@DESKTOP-EVK789N:~$ sudo apt-get install docker-ce=18.06.1~ce~3-0~ubuntu docker-ce-cli=18.06.1~ce~3-0~ubuntu containerd.io
Reading package lists... Done
Building dependency tree
Reading state information... Done
E: Version '18.06.1~ce~3-0~ubuntu' for 'docker-ce' was not found
E: Version '18.06.1~ce~3-0~ubuntu' for 'docker-ce-cli' was not found
shih@DESKTOP-EVK789N:~$ sudo docker run hello-world
docker: Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?.
See 'docker run --help'.
shih@DESKTOP-EVK789N:~$ curl -fsSL https://get.docker.com -o get-docker.sh
shih@DESKTOP-EVK789N:~$ DRY_RUN=1 sh ./get-docker.sh
# Executing docker install script, commit: 93d2499759296ac1f9c510605fef85052a2c32be
Warning: the "docker" command appears to already exist on this system.

If you already have Docker installed, this script can cause trouble, which is
why we're displaying this warning and provide the opportunity to cancel the
installation.

If you installed the current Docker package using this script and are using it
again to update Docker, you can safely ignore this message.

You may press Ctrl+C now to abort this script.
+ sleep 20
^C
shih@DESKTOP-EVK789N:~$ ./get-docker.sh
-bash: ./get-docker.sh: Permission denied
shih@DESKTOP-EVK789N:~$ curl -fsSL https://get.docker.com -o get-docker.sh
shih@DESKTOP-EVK789N:~$ sudo sh get-docker.sh
# Executing docker install script, commit: 93d2499759296ac1f9c510605fef85052a2c32be
Warning: the "docker" command appears to already exist on this system.

If you already have Docker installed, this script can cause trouble, which is
why we're displaying this warning and provide the opportunity to cancel the
installation.

If you installed the current Docker package using this script and are using it
again to update Docker, you can safely ignore this message.

You may press Ctrl+C now to abort this script.
+ sleep 20


WSL DETECTED: We recommend using Docker Desktop for Windows.
Please get Docker Desktop from https://www.docker.com/products/docker-desktop


You may press Ctrl+C now to abort this script.
+ sleep 20
+ sh -c apt-get update -qq >/dev/null
W: Target Packages (stable/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Translations (stable/i18n/Translation-en) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-amd64) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-all) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Translations (stable/i18n/Translation-en) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-amd64) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-all) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
+ sh -c DEBIAN_FRONTEND=noninteractive apt-get install -y -qq apt-transport-https ca-certificates curl >/dev/null
+ sh -c curl -fsSL "https://download.docker.com/linux/ubuntu/gpg" | gpg --dearmor --yes -o /usr/share/keyrings/docker-archive-keyring.gpg
+ sh -c echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu focal stable" > /etc/apt/sources.list.d/docker.list
+ sh -c apt-get update -qq >/dev/null
W: Target Packages (stable/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Translations (stable/i18n/Translation-en) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-amd64) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-all) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-amd64/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Packages (stable/binary-all/Packages) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target Translations (stable/i18n/Translation-en) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-amd64) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
W: Target CNF (stable/cnf/Commands-all) is configured multiple times in /etc/apt/sources.list:50 and /etc/apt/sources.list.d/docker.list:1
+ sh -c DEBIAN_FRONTEND=noninteractive apt-get install -y -qq --no-install-recommends  docker-ce-cli docker-scan-plugin docker-ce >/dev/null
+ version_gte 20.10
+ [ -z  ]
+ return 0
+ sh -c DEBIAN_FRONTEND=noninteractive apt-get install -y -qq docker-ce-rootless-extras >/dev/null

================================================================================

To run Docker as a non-privileged user, consider setting up the
Docker daemon in rootless mode for your user:

    dockerd-rootless-setuptool.sh install

Visit https://docs.docker.com/go/rootless/ to learn about rootless mode.


To run the Docker daemon as a fully privileged service, but granting non-root
users access, refer to https://docs.docker.com/go/daemon-access/

WARNING: Access to the remote API on a privileged Docker daemon is equivalent
         to root access on the host. Refer to the 'Docker daemon attack surface'
         documentation for details: https://docs.docker.com/go/attack-surface/

================================================================================

shih@DESKTOP-EVK789N:~$
shih@DESKTOP-EVK789N:~$ sudo docker run hello-world
docker: Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?.
See 'docker run --help'.
shih@DESKTOP-EVK789N:~$ sudo service docker status
 * Docker is not running
shih@DESKTOP-EVK789N:~$
```
---
```
Windows PowerShell
著作權（C） Microsoft Corporation。保留擁有權利。

安裝最新的 PowerShell 以取得新功能和改進功能！https://aka.ms/PSWindows

PS C:\Windows\system32> wsl --list
Windows 子系統 Linux 版發佈:
Ubuntu (預設值)
PS C:\Windows\system32> wsl --list --online
以下是可安裝之有效發佈的清單。
使用 'wsl --install -d <Distro>' 安裝。

NAME            FRIENDLY NAME
Ubuntu          Ubuntu
Debian          Debian GNU/Linux
kali-linux      Kali Linux Rolling
openSUSE-42     openSUSE Leap 42
SLES-12         SUSE Linux Enterprise Server v12
Ubuntu-16.04    Ubuntu 16.04 LTS
Ubuntu-18.04    Ubuntu 18.04 LTS
Ubuntu-20.04    Ubuntu 20.04 LTS
PS C:\Windows\system32> wsl --install -d Kali-Linux
正在下載：Kali Linux Rolling
正在安裝：Kali Linux Rolling
已完成安裝 Kali Linux Rolling。
正在啟動 Kali Linux Rolling...
PS C:\Windows\system32>
```


---
https://pureinfotech.com/install-ubuntu-windows-10/
https://pureinfotech.com/install-wsl-windows-11/
https://iter01.com/610179.html

在 windows terminal 視窗中，輸入如下指令來啟用 WSL 服務：

開啟linux子系統
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

開啟虛擬機器平臺
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart



開啟方式2-圖形化
按下 Win + R，調出命令輸入視窗。輸入指令 appwiz.cpl。

點選左側的 【啟動或關閉 Windows 功能】：

---
https://iter01.com/610179.html
需要勾選【適用於 Linux 的 Windows 子系統】和【虛擬機器平臺】這兩項。

接下來要做的事情，就是安裝 Ubuntu 作業系統。

設定WSL的版本為WSL2
$ wsl --set-default-version 2
執行更新wsl命令已確認wsl為最新版
$ wsl --update
wsl&nbsp;--install // 安裝wslg

檢視可安裝版本
$ wsl --list --online // 列出所有可安裝的linux版本
開始安裝
$ wsl --install -d Ubuntu-20.04 // 安裝Ubuntu-20.04

安裝方式2-圖形化（windows store）
啟動 【Windows Store】並搜尋 Ubuntu，然後選擇要安裝的系統

安裝完成之後，點選【啟動】按鈕

第一次開啟速度稍微慢一些，大約 1 分鐘左右吧，提示設定使用者名稱、密碼，然後就進入我們熟悉的視窗了

安裝GUI程式並測試
sudo apt update
sudo apt upgrade
sudo apt install gedit // gnome桌面下的編輯器

命令執行完成功後會在開始選單下生成Ubuntu-20.04

---
## uninstall WSL2
https://pureinfotech.com/uninstall-wsl2-windows-10/

1. Open Settings on Windows 10.

2. Click on Apps.

3. Click on Apps & features.

4. Select the distribution of Linux and click the Uninstall button.

5. Click the Uninstall button again.

---
WSL uninstall

WSL 2 是否使用 Hyper-V？ 是否可在 Windows 10 家用版上使用？
wsl2 install windows 11
什麼是 WSL
WSL(Windows Subsystem for Linux)：Windows 系統中的一個子系統，在這個子系統上可以執行 Linux 作業系統。
WSL： 並不是一個真正的 Linux 作業系統，僅僅是 Linux 應用程式與 Windows 作業系統之間的一個適配層。

在這個適配層之上，可以執行 Linux 應用程式，有點類似於以前的 cygwin 的方式。

WSL2：它就是一個虛擬機器，類似於 Vitual Box，在這個虛擬機器之上，執行一個完整的 Linux 作業系統。

相對於 Virtual Box、VMWare 來說，WSL2提供更全面的相容性、與 Windows 系統的互操作性更好、執行速度更快、佔用系統資源更少。

## 如何在 Windows 11 上安裝適用於 Linux 的 Windows 子系統 (WSL)
https://setupbits.com/zh-hant/%E5%A6%82%E4%BD%95%E5%9C%A8-windows-11-%E4%B8%8A%E5%AE%89%E8%A3%9D%E9%81%A9%E7%94%A8%E6%96%BC-linux-%E7%9A%84-windows-%E5%AD%90%E7%B3%BB%E7%B5%B1-wsl

在windows 11中安裝WSLG(WSL2)
https://iter01.com/610179.html



將版本從 WSL 1 升級至 WSL 2
https://docs.microsoft.com/zh-tw/windows/wsl/install
$ wsl --set-version <distro name> 2<distro name>
$ wsl --set-version Ubuntu-20.04 2

從 Microsoft Store 安裝 WSL
您還可以從 Microsoft Store 下載打包到應用程序中的所有組件。 使用這種方法的好處是該功能將獨立於 Windows 11 運行，並且可以通過 Microsoft Store 獲得更新，而無需等待操作系統的下一個版本安裝最新版本。

要從 Microsoft Store 安裝 WSL，請使用以下步驟：

1. 啟用虛擬機平台
    1. 打開 Start.

    2. 搜索 Turn Windows Features on or off 並單擊頂部結果以打開頁面。

    3. 檢查 Virtual Machine Platform.

    虛擬機平台

    4. 點擊 OK.

    5. 點擊 Restart.

完成這些步驟後，您可以繼續從 Microsoft Store 下載該應用程序。

2. 下載適用於 Linux 的 Windows 子系統應用程序
    1. 打開 Windows Subsystem for Linux 頁.

    2. 點擊 Get.

    3. 點擊 Open.

    4. 點擊 Get.

Microsoft Store WSL 安裝

完成這些步驟後，WSL 將安裝在 Windows 11 上，包括對 Linux GUI 應用程序的支持。

我們可能會使用我們的鏈接賺取購買佣金，以幫助繼續提供免費內容。 隱私政策信息。

本網站上的所有內容均不提供任何明示或暗示的保證。 Use any information at your own risk. 在進行任何更改之前，請務必備份您的設備和文件。 隱私政策信息。




在 Windows 11 上安裝 WSL
1. 打開 Start 在 Windows 11 上。

2. 搜索 Command Prompt, 右鍵單擊頂部結果，然後選擇 Run as administrator.

3. 鍵入以下命令以 在 Windows 11 上安裝 WSL 並按下 Enter：

$ wsl --install

4. 重新啟動計算機以完成 Windows 11 上的 WSL 安裝。

5. 根據需要繼續進行 Linux 發行版設置。

Windows 11 上使用特定發行版安裝 WSL

1. 打開 Start.

2. 搜索 Command Prompt, 右鍵單擊頂部結果，然後選擇 Run as administrator.

3. 鍵入以下命令以查看可以在 Windows 11 上安裝的可用 WSL 發行版列表，然後按 Enter：
    $ wsl --list --online
        Quick note: 在撰寫本文時，您可以安裝 Ubuntu、Debian、Kali Linux、openSUSE 和 SUSE Linux Enterprise Server。

4. 輸入以下命令安裝 Windows 11 上具有特定發行版的 WSL 並按下 Enter：
    $ wsl --install -d DISTRO-NAME
        DISTRO-NAME 對於您要安裝的發行版的名稱，例如 Debian.

5. 重新啟動計算機以完成 Windows 11 上的 WSL 安裝。

6. 根據需要繼續進行 Linux 發行版設置。

完成這些步驟後，Windows Subsystem for Linux 2 組件將與您指定的 Linux 發行版一起安裝。

在 Windows 11 上更新 WSL 內核
要使用命令提示符將 WSL 內核更新到最新版本，請使用以下步驟：

1. 打開 Start.

2. 搜索 Command Prompt, 右鍵單擊頂部結果，然後選擇 Run as administrator.

3. 鍵入以下命令以 在 Windows 11 上更新 WSL 內核 並按下 Enter：

    $ wsl --updateCopy

完成這些步驟後，如果有可用更新，它將下載並安裝到您的計算機上。



Uninstall WSL2 on Windows 10

https://pureinfotech.com/uninstall-wsl2-windows-10/

download docker toolbox for windows

docker run hello-world

https://dockereasytoturial.gitbook.io/docker_tutorial_in_30mins/get_started/helloworld

https://melayogu.pixnet.net/blog/post/336029260-%5Bubuntu%5D-docker-run-hello-world

https://docs.microsoft.com/zh-tw/windows/wsl/tutorials/wsl-containers

https://openhome.cc/Gossip/CodeData/DockerLayman/DockerLayman1.html

https://www.runoob.com/docker/windows-docker-install.html

https://dockerlabs.collabnix.com/beginners/helloworld/

https://hub.docker.com/_/hello-world

https://github.com/docker-library/hello-world

https://ithelp.ithome.com.tw/articles/10238216

https://ithelp.ithome.com.tw/articles/10202089

https://matthung0807.blogspot.com/2019/12/docker-run-hello-world-image.html









https://hub.docker.com/_/python

https://github.com/docker-library/hello-world

https://docs.docker.com/language/python/build-images/

https://docs.docker.com/desktop/windows/install/
https://docs.docker.com/desktop/windows/install/

https://docs.docker.com/desktop/windows/

https://www.codebuug.com/cs115347807/

https://www.codebuug.com/cs115347807/


https://docs.microsoft.com/zh-tw/windows/wsl/install
$ wsl --install -d ubuntu

https://docs.microsoft.com/zh-tw/windows/wsl/install

https://docs.microsoft.com/zh-tw/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package

https://docs.microsoft.com/zh-tw/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package


http://mirrors.aliyun.com/docker-toolbox/windows/docker-toolbox/

https://stackoverflow.com/questions/40459280/docker-cannot-start-on-windows

HTML URL Encoding Reference
https://www.w3schools.com/tags/ref_urlencode.ASP


https://stackoverflow.com/questions/40459280/docker-cannot-start-on-windows



## 123

    Docker
    Windows 
    Windows Hyper-V
    Linux
    Linux
    iOS
    VB
    Topic branch
    Linux
    建立與使用image
    
### 指令
    pull
    images
    run
    ps
    stop
    start
    exec
    commit
    tag
    rmi
    rm
    push

## 指令2
    映像檔 Image
    容器 Container
    run、start、stop、rm
    ### 倉庫 Registry
    docker search nginx
    docker version
    docker info
    docker pull ubuntu
    Docker 列出 Local Images
    docker images
    Docker 啟動 Image 產生 Container
    docker start hash-id
    Docker 暫停 Image
    docker stop hash-id
    Docker 執行 Image
    docker run -d debian:jessie
    Docker 執行 Container
    docker exec hash-id /sbin/ifconfig
    Docker 掛載目錄進入 Container
    docker -v 掛載點
    docker run -d --name xxx -p 80:80 -p 3306:3306 -v /mnt/xxx:/mnt debian:jessie
    Docker 產生、操作 Volumes
    docker volume create --name myvol # 建立 local volume
    docker run -v myvol:/data # Container start 就 Mount 此 volume
    Docker 列出 Container
    docker ps # 還在執行中的 Container，可以看到詳細 hash id
    docker ps -a # 執行、停止的 Container 都列出來
    Docker 進入(Attach) Container
    docker attach hash-id
    Docker 列出 Logs
    docker logs hash-id
    Docker 刪除 Container
    docker rm -f hash-id # 強置刪除
    Docker 刪除 Images
    docker rmi image-id
    docker rmi -f image-id # 強置刪除

    https://docs.docker.com/engine/reference/commandline/docker/

### 安装 
    https://www.runoob.com/docker/docker-build-command.html
    Ubuntu
    Debian 
    CentOS 
    Windows 
    MacOS
    
### 使用
    docker run ubuntu:15.10 /bin/echo "Hello world"
    docker stats --help
    docker pull ubuntu
    docker run -it ubuntu /bin/bash
    docker ps -a
    docker start b750bbbcfd88
    docker run -itd --name ubuntu-test ubuntu /bin/bash
    docker stop <容器 ID>
    docker restart <容器 ID>
    docker attach 1e560fca3906 
    docker exec -it 243c32535da7 /bin/bash
    docker export 1e560fca3906 > ubuntu.tar
    docker import http://example.com/exampleimage.tgz example/imagerepo
    docker rm -f 1e560fca3906
    docker pull training/webapp  # 载入镜像
    docker run -d -P training/webapp python app.py
    docker ps
    docker port bf08b7f2cd89
    docker logs -f bf08b7f2cd89
    docker rm wizardly_chandrasekhar  

### 镜像使用
    docker images
    docker run -t -i ubuntu:15.10 /bin/bash
    docker pull ubuntu:13.10
    docker search httpd
    docker pull httpd
    docker run httpd
    docker rmi hello-world

### 容器连接
    创建了一个 python 应用的容器
        docker run -d -P training/webapp python app.py
        docker ps
        docker run -d -p 127.0.0.1:5001:5000 training/webapp python app.py
    
### 仓库管理
    docker login
    docker logout
    docker search ubuntu
    
### 網站資源
    Docker 教程 https://www.runoob.com/docker/docker-tutorial.html
    Docker 初學筆記 - 基本指令操作教學 https://blog.longwin.com.tw/2017/01/docker-learn-initial-command-cheat-sheet-2017/
    Docker CLI https://docs.docker.com/engine/reference/commandline/docker/
    用30天來介紹和使用 Docker https://ithelp.ithome.com.tw/users/20103456/ironman/1320
    Docker學習筆記 
    Get started with Docker for Windows https://docs.docker.com/docker-for-windows/
 

### 流程
    1.建立自己的 code
    2.寫入Dockerfile
    3.建立images
    4.定義services
    5.run containers
    6.test My code
    7.git push
