## Supervisor Dockerfile

This repository contains **Dockerfile** of [Supervisor](http://supervisord.org/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/darkterra/supervisor-docker/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).

### Base Docker Image

* [darkterra/supervisor-docker](https://hub.docker.com/r/darkterra/supervisor-docker/)

### Installation

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/darkterra/supervisor-docker/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull darkterra/supervisor-docker`

   (alternatively, you can build an image from Dockerfile: `docker build -t="darkterra/supervisor-docker" https://github.com/darkterra/supervisor-docker`)

### Usage

    docker run -it --rm darkterra/supervisor-docker

#### Run with custom config directory

    docker run -d -v <config-dir>:/etc/supervisor/conf.d darkterra/supervisor-docker