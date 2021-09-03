follow the commands to build run and push \
```
$ docker build --tag api_server .
```
```
$ docker run -p 8081:8081 api_server
```
```
$ docker tag api_server tasdidur/go_api_server
```
```
$ docker push tasdidur/go_api_server
```
