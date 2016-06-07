# docker-images-ubuntu-extended
Extended base Docker images for Ubuntu

## Why?
Ubuntu base docker images are pretty restricted. They don't include some packages which I deem
quite necessary and useful even in a simple image; I just add those packages.

This image includes [su-exec](https://github.com/ncopa/su-exec) and [apt-current](https://github.com/alanfranz/apt-current), along
other packages that you can find in each [Dockerfile](trusty/Dockerfile)

You can use this image straight from docker hub: [alanfranz/ubuntu-extended:trusty](https://hub.docker.com/r/alanfranz/ubuntu-extended/)
