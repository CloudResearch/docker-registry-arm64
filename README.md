# Docker registry ARM64

Docker registry build for ARM64. Based on [budry/registry-arm](https://hub.docker.com/r/budry/registry-arm/), thank you for your amazing work!

This package is based on official [docker registry](https://github.com/docker/distribution-library-image/)

## Content

* [The why?](#Why?)
* [What to do?](#What-to-do?)
* [How to use](#how-to-use)
    * [Docker](#docker)

## Why?

This package was developed for running docker registry on ARM64 devices. Builder image is based on arm64v8/golang and final registry image is based upon arm64v8/debian.


## What to do?

This image is build for ARM64. Based on the original distribution package.  
1. Just follow the official configuration guide: https://docs.docker.com/registry/deploying/
2. Use "bl4ckbird/registry-arm64" in your docker-compose.yml

Used and tested on ARM64 [scaleway](http://scaleway.com) instance

## How to use 


### Docker 

You can use my build of this package with name 

```shell
$ docker run -d -p 5000:5000 --restart always bl4ckbird/registry-arm64
```

