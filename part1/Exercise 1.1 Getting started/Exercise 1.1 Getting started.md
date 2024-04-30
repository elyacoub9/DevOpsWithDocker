```markdown
[root@localhost ~]# docker stop 9b bf

9b
bf

[root@localhost ~]# docker ps -a
CONTAINER ID   IMAGE     COMMAND                  CREATED              STATUS                     PORTS     NAMES
9bf0cabc6009   nginx     "/docker-entrypoint.…"   46 seconds ago       Exited (0) 3 seconds ago             practical_mestorf
bf72baa93e19   nginx     "/docker-entrypoint.…"   51 seconds ago       Exited (0) 3 seconds ago             frosty_morse
40fb083dbde3   nginx     "/docker-entrypoint.…"   About a minute ago   Up About a minute          80/tcp    gracious_lehmann
```