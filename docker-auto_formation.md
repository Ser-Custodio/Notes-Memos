# DOCKER

## Container
1. Holds things: Something is either inside the container or outside the container
2. Is portable: It can be used on the local machine, a coworker's machine or a cloud
3. Has clear interfaces for access: It has ports that can be opened for inteacting through the browser or interact with data through the command line
4. Can be obtained from a remote location: An offsite **registry** keeps an image (which is a mold) for your container

## Image
Docker images are like blueprints or molds. They are immutable master templates to create our containers.

## Dockerfile
File that refers to a base image that is used to build the initial layer of the container.
Is a set of instructions to build the container as we want it.

## Docker Essentials

### Docker Platform
Docker software that provids the ability to package and run applications in a container on any server. It bundles code files and dependencies and promotes easy scaling by enabling portability and reproducibility.

### Docker Engine
Client-server application. 

### Docker Daemon
Docker server that listens for Docker API requests, it manages images, containers, networks and volumes.

### Docker Volumes
Way of storing the persistent data that the app consumes and creates.

### Docker Registry
Remote location where the images are stored. You push images to a registry and you pull images from a registry.

### Docker repository
Collection of Docker images with the same name and different tags. _Tags_ are the identifiers of an image.

Usually a repository has different versions of the same image. For example, Python is the name of the most popular official Docker image repository on Docker Hub. Python:3.7-slim refers to the version of the image with the 3.7-slim tag in the Python repository.

## Scaling Docker
Using multiple containers at once

### Docker Networking
It allows to connect Docker containers together.
Connected Docker containers can be on the same host or multiple hosts.

![Docker Networking](images/docker/Docker_Network.png)

There are 4 modes available for Docker Networking: _Bridge, Host, Container_ or _no networking_.

You can check the detail [here](docker_networking.md)