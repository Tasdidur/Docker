# Docker
useful links : \
https://www.freecodecamp.org/news/a-beginners-guide-to-docker-how-to-create-your-first-docker-application-cc03de9b639f/ \
https://www.callicoder.com/docker-golang-image-container-example/ \
https://nickjanetakis.com/blog/tag/docker-tips-tricks-and-tutorials \
\
useful commands : 

List your images.
```
$ docker image ls
```
\
Delete a specific image.
```
$ docker image rm [image name]
```
\
Delete all existing images.
```
$ docker image rm $(docker images -a -q)
```
\
List all existing containers (running and not running).
```
$ docker ps -a
```
\
Stop a specific container.
```
$ docker stop [container name]
```
\
Stop all running containers.
```
$ docker stop $(docker ps -a -q)
```
\
Delete a specific container (only if stopped).
```
$ docker rm [container name]
```
\
Delete all containers (only if stopped).
```
$ docker rm $(docker ps -a -q)
```
\
Display logs of a container.
```
$ docker logs [container name]
```
