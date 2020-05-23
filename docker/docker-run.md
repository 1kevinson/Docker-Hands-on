<!-- @format -->
## Docker run commands

---

__docker run__

_It's use to run a container from and image, first it's try to find image locally, if there's no image,then it's downloads it from dockerhub._

__GOOD TO KNOW__ : Container only run if it's have a task running inside, that's why we run bash with centos container ( if there is no task running container will automatically stop )
> docker run centos

_Docker container Id_

-[root@3c21189545df /]#   ----> `3c21189545df` is the unique Id of the docker container

login in the container once it's run (-it) and execute the bash command to open the terminal in the container
> docker run -it centos bash

run a command in a container (get the os version)
> docker run ubuntu cat /etc/os-release

run container in background (-d) & sleep the os after 20s (sleep 20)

__GOOD TO KNOW__ : **for every task**, docker create a new instance of image (container)
> docker run -d centos sleep 20

run container with tag (version), if it's no tag setted docker use the default tag
> docker run redis:4.0

run container and map his port with the host port (cannot map when the container is running)
> docker run -p `hostPort`:`containerPort` -d nginx

> docker run -p 8000:80 -d nginx

_then go back to the browser and open with localhost (host) 127.0.0.1:8080_