## Go Dockerfile

This repository contains a **Dockerfile** to create a docker base image with latest version of Go programming language 

This **Dockerfile** has been published as a [trusted build](https://index.docker.io/u/jamesdbloom/docker_java7_maven/) to the public [Docker Registry](https://index.docker.io/).


### Dependencies

* [ubuntu](http://dockerfile.github.io/#/ubuntu)


### Installation

1. Install [Docker](https://www.docker.io/).

2. Download [trusted build](https://index.docker.io/u/samirabloom/docker-go/) from public [Docker Registry](https://index.docker.io/): `docker pull samirabloom/docker-go`

   (alternatively, you can build an image from Dockerfile: `docker build -t="samirabloom/docker-go" github.com/samirabloom/docker-go`)


### Usage (two options)

#### 1. Run container and clone git repo into container

    docker run -i -t -name docker_go -rm samirabloom/docker-go

    git clone <your repo url>

#### 2. Run container with git repo attached container (from host OS)

    docker run -i -t -name docker_go -rm -v <your git repo directory>:/volume/git samirabloom/docker-go
    
<a href="https://github.com/samirarabbanian">Samira Bloom</a>