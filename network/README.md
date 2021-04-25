# Docker networks

## Default docker bridge

```docker
docker run -dit --name alpine1 alpine ash

docker run -dit --name alpine2 alpine ash

docker network inspect bridge
```

## User-defined bridge networks

### Network creation

```docker
docker network create --driver bridge alpine-net

docker network inspect alpine-net
```

### Test containers

```docker
docker run -dit --name alpine1 --network alpine-net alpine ash

docker run -dit --name alpine2 --network alpine-net alpine ash

docker run -dit --name alpine3 alpine ash

docker run -dit --name alpine4 --network alpine-net alpine ash

docker network connect bridge alpine4
```
