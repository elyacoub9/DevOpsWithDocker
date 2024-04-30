```console
[root@localhost Exercise 1.9]# touch text.log

[root@localhost Exercise 1.9]# docker run -d -v "$(pwd)/text.log:/usr/src/app/text.log" devopsdockeruh/simple-web-service
cb6d686c3c722d2bf409362ec5ec45b50066f9a0b73716245e951b3ffb8a45f5
[root@localhost Exercise 1.9]# ls
text.log

[root@localhost Exercise 1.9]# cat text.log
2024-04-29 11:08:24 +0000 UTC
2024-04-29 11:08:26 +0000 UTC
2024-04-29 11:08:28 +0000 UTC
2024-04-29 11:08:30 +0000 UTC
2024-04-29 11:08:32 +0000 UTC
Secret message is: 'You can find the source code here: https://github.com/docker-hy'
2024-04-29 11:08:34 +0000 UTC

[root@localhost Exercise 1.9]# docker ps
CONTAINER ID   IMAGE                               COMMAND                 CREATED          STATUS          PORTS     NAMES
cb6d686c3c72   devopsdockeruh/simple-web-service   "/usr/src/app/server"   29 seconds ago   Up 28 seconds             recursing_montalcini

[root@localhost Exercise 1.9]# docker stop cb
cb
```