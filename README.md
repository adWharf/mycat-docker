
[![Docker Stars](https://img.shields.io/docker/stars/williamwxl/mycat.svg)](https://hub.docker.com/r/williamwxl/mycat/)


[![Docker Pulls](https://img.shields.io/docker/pulls/williamwxl/mycat.svg)](https://hub.docker.com/r/williamwxl/mycat/)


[![Docker Automated build](https://img.shields.io/docker/automated/williamwxl/mycat.svg)](https://hub.docker.com/r/williamwxl/mycat/)


[![Docker Build Status](https://img.shields.io/docker/build/williamwxl/mycat.svg)](https://hub.docker.com/r/williamwxl/mycat/)


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
