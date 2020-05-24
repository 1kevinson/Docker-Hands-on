<!-- @format -->

## Docker general commands

---
_If you install docker desktop for mac then macbook becomesthe docker host_


Get the ip address of a container

> docker inspect `conid` | grep "IPAddress" 

Search the docker hub for image ( with limit option)

> docker search --limit 10 timer

Always check there for good stuff 👇🏽

[Docker-cli Reference](https://docs.docker.com/engine/reference/commandline/cli/)


The ENTRYPOINT in docker file is the command to run the application