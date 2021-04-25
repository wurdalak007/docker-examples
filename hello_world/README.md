# The simplest dockerfile

To see containers

```docker
docker ps -- launched containers

docker ps -a -- all containers

docker container rm $(docker ps -q -a) -- to remove all stopped containers
```

```docker
docker build -t hello-world .

docker run --name hello hello-world
```

To remove stopped container use --rm option:

```docker
docker run --rm --name hello hello-world
```
