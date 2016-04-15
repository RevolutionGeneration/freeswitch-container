FreeSWITCH Dockerfile
=====================

This project can be used to deploy a FreeSWITCH server inside a Docker container

## Start

```
 docker run \
  -h node1.example.com \
  -tid \
  -v /path/to/erlang.cookie:/etc/freeswitch/.erlang.cookie:ro \
  -p 11000:11000 \
  -p 8021:8021 \
  revgen/freeswitch-container \
  /bin/bash
``` 