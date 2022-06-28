# docker
- Memcached
```
docker run --name memcached -it --rm -p 11211:11211 docker.io/bitnami/memcached:1
```
- Redis
```
docker run --name nbm-redis -p  6379:6379 redis
docker run --name redis -d -p 6379:6379 redis redis-server --requirepass "8gNR#9V2}[<W"
```
- Mysql
```
docker run --name mysql-ecommercedev -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=ecommercedev -p 3308:3306 mysql:5.7.36
```

- Portainer
```
docker volume create portainer_data
docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:latest
```
