# H2O in Docker

[![Docker Pulls](https://img.shields.io/docker/pulls/frosner/h2o.svg?maxAge=2592000)](https://hub.docker.com/r/frosner/h2o/)
[![](https://images.microbadger.com/badges/image/frosner/h2o.svg)](https://microbadger.com/images/frosner/h2o "Get your own image badge on microbadger.com")

## Usage

```
docker run \
  --net host \
  -e H2O_NODE_COUNT=1 \
  -e H2O_GROUP_ID=1100 \
  -e H2O_USER_ID=1100 \
  frosner/h2o \
  java \
  -Xmx1g \
  -jar /opt/h2o.jar \
  -name "h2o-cluster" \
  -nthreads 2
```
