# Ports forwarding and volumes demo

```docker
docker build -t hello-world .

docker run --name hello hello-world
```

To remove stopped container use --rm option:

```
docker run --rm --name hello hello-world
```