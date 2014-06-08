docker-haproxy
==============

This is part of [mayfly](https://github.com/bewt85/mayfly) which demonstrates the 
concept of testing groups of versions of services in short lived virtual environments.

This is a docker container which uses incrond to reload itself whenever haproxy.cfg changes.
It is updated by [haproxy_updater](https://github.com/bewt85/mayfly-haproxy-updater) which
mounts the `/etc/haproxy` folder.

You can build your own version of the container by setting the following environment variable 
to your docker index username (if you don't it uses mine) and running this bash script:

```
export DOCKER_ACCOUNT_NAME=<your_name>
sudo -E ./build.sh
```
