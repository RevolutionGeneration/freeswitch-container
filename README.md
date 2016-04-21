FreeSWITCH Dockerfile
=====================

This project can be used to deploy a FreeSWITCH server inside a Docker container

## Start

```
docker run \
  -tid \
  --net=host \
  -h n1.wdcloud.eu \
  -v /root/.erlang.cookie:/etc/freeswitch/.erlang.cookie \ 
  --name freeswitch \
  revgen/freeswitch-container \ 
  /bin/bash
  
``` 