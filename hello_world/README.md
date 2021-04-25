# Ports forwarding and volumes demo

```docker
docker build -t hello-world .

docker run --name web-app python-example
```

To remove stopped container use --rm option:

```
docker run --rm --name web-app python-example
```