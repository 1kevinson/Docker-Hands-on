<!-- @format -->

## Docker containers commands

---

start container with name or container Id 

> docker start `name_or_id`

stop container with name or container Id (exit code 137)

> docker stop `name`

> docker stop `id`

kill container with name or container Id 

> docker kill `name_or_id`

restart container with name or container Id 

> docker restart `name_or_id`

suspend container with name or container Id 

> docker pause `name_or_id`

resume  container with name or container Id 

> docker unpause `name_or_id`

remove containers with name or container Id

> docker rm `conId`

> docker rm `conId` `conId` `conId`

attach to a running container (stdin/stdout/sterr)

> docker attach `name`

logs container (container outputs)

> docker logs `name`

inspect container (show low-level infos)

> docker inspect `name`

docker container ip address

> docker inspect --format '{{ .NetworkSettings.IPAddress }}'` container_name_or_id`

execute a command on a running container

> docker exec `conId` cat /etc/os-release


