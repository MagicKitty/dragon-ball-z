# 1 - Introduction à Docker

### Docker

```bash
sudo docker run hello-world

sudo docker container run -itd --name=hello alpine /bin/sh

sudo docker exec hello /bin/sh -c "echo "Welcome to DBZ!" > hello.txt"

sudo docker exec hello cat hello.txt

sudo docker run mysql
sudo docker run postgres

sudo docker rm -f $(sudo docker container ls -aq) # on peut enlever le flag --force pour ne pas supprimer les conteneurs qui sont en cours d'exécution
```

### Tomcat/Nginx

```bash
sudo docker run -d -p 9876:8080 tomcat

sudo docker run -d -p 9875:80 nginx:alpine

sudo docker run -d -p 9875:80 -v $(pwd)/index.html:/usr/share/nginx/html/index.html nginx:alpine
```


