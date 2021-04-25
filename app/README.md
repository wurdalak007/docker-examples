# Ports forwarding and volumes demo

```docker
docker build -t python-example .

docker run --rm -p 8080:8080 --name web-app python-example

docker run --rm -p 8080:8080 -v <host-path-to-repo>/docker-examples/app/resources:/usr/src/app/resources --name web-app python-example
```
