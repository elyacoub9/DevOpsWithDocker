
-  commands

```
[root@localhost ~]# docker run -dit --name secret_message devopsdockeruh/simple-web-service:ubuntu
5810e62082749792fab8091ba5b14e34625ec6d64260b4c69ba300dfb587e361

[root@localhost ~]# docker exec secret_message tail -f ./text.log
```

-  the secret message

```
'You can find the source code here: https://github.com/docker-hy'
``` 