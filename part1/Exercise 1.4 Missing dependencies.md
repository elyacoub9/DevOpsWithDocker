- one comamnd 

```bash
[root@localhost ~]# docker run -it --rm --name missing_dependencies ubuntu  sh -c ' apt update && apt install curl -y && while true; do echo "Input website:
"; read website; echo "Searching.."; sleep 1; curl http://$website; done'
```
-  to fix the ensuing problem
```bash
apt update && apt install curl -y
```

- output
```bash
Input website:
helsinki.fi
Searching..
<html>
<head><title>301 Moved Permanently</title></head>
<body>
<center><h1>301 Moved Permanently</h1></center>
<hr><center>nginx/1.22.1</center>
</body>
</html>
Input website:
```
