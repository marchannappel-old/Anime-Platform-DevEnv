FROM jenkins/jenkins:lts

MAINTAINER "Marc Hannappel"

ARG DOCKER_VERSION=1.13.1

USER root

RUN curl -fsSL https://get.docker.com/builds/Linux/x86_64/docker-$DOCKER_VERSION.tgs \
    | tar --strip-components=1 -xz -C /usr/local/bin docker/docker

# Run docker container with: docker container run -d --name jenkins-master -p 8080:8080 -p 50000:50000 \
# -v ~/jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock \
# my-jenkins-docker-cli:lts

# docker exec -ti jenkins-master /bin/bash
