# mycat-docker
Dockerfile for [MyCat](https://github.com/MyCATApache/Mycat-Server)

The image is available directly from [Docker Hub](https://hub.docker.com/r/williamwxl/mycat/)

# Simple Tags

- `master` `1.6-slim` [(1.6-slim)](https://github.com/adWharf/mycat-docker/tree/master/1.6-slim)

# Usage

```
docker run \
    -v /my/path/of/logs:/opt/mycat/logs \
    -v myschema.xml:/opt/mycat/conf/schemal.xml \
    -v myserver.xml:/opt/mycat/conf/server.xml \
    -v myrules.xml:/opt/mycat/conf/server.xml \
    -p 3306:3306 \
    williamwxl/mycat
```
