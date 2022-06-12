# docker
- Memcached
```
docker run --name memcached -it --rm -p 11211:11211 docker.io/bitnami/memcached:1
```
- Redis
```
docker run --name nbm-redis -p  6379:6379 redis
```
- Mysql
```
docker run --name mysql-ecommercedev -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=ecommercedev -p 3308:3306 mysql:5.7.36
```
