- compare the image sizes 
```conole
[root@localhost ~]# docker image ls | grep devopsdockeruh
devopsdockeruh/simple-web-service   ubuntu    4e3362e907d5   3 years ago   83MB
devopsdockeruh/simple-web-service   alpine    fd312adc88e0   3 years ago   15.7MB
```
- secret message 
```console
[root@localhost ~]# docker run -dit --name devopsdockeruh_alpine1 devopsdockeruh/simple-web-service:alpine
```
```console
[root@localhost ~]# docker exec devopsdockeruh_alpine tail -f ./text.log
2024-04-28 17:14:29 +0000 UTC
2024-04-28 17:14:31 +0000 UTC
2024-04-28 17:14:33 +0000 UTC
2024-04-28 17:14:35 +0000 UTC
2024-04-28 17:14:37 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
```
