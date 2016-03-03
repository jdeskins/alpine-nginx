# alpine-nginx

Run nginx in Alpine Docker container with total size around 7MB.

Build the image:

```
docker build -t alpine-nginx .
```

Run in daemon mode on port 80 of host.

```
docker run -d -p 80:8080 alpine-nginx
```

View nginx running on host http://localhost

If running docker-machine, you can launch in default browser by running:

```
open http://${docker-machine ip default}
```

View the running processes of the container:

```
docker exec [CONTAINER_NAME] ps
```
