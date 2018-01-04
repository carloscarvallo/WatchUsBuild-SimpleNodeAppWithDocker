# WatchUsBuild-SimpleNodeAppWithDocker
Watch Us Build code for the Simple Node App With Docker screencast.

## Cheatsheet

``` bash
$ docker info
$ docker
$ docker pull nginx
$ docker container run nginx:latest
# without name
$ docker container run -p 9999:80 nginx:latest
$ docker container run -p 9999:80 --name web-server nginx:latest
# doing a map from the root so to the container
$ docker container run -p 9999:80 --name web-server --rm -v /Users/carloscarvallo/dev/screencasts/nodeapp-with-docker/nginx/html:/usr/share/nginx/html nginx:latest
# build from a Dockerfile
$ docker build -t web-server .
$ docker image ls
$ docker container run --name web-server --rm -p 9999:80 web-server:latest
# stop a docker container
$ docker stop web-server
# list all images
$ docker images -a
# delete a image
$ docker rmi 4a2c3aa6e871
# example of entering to docker prompt
$ docker container exec -it node-db psql -U postgres
# inspect docker network
$ docker network inspect bridge
# see docker containers running
$ docker container ps
```
