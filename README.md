# Docker

## Monolithic vs Microservices
Monolithic :-
A monolithic application is a single tired software application in which all components are combined into one program from a single 
platform.

Microservices :-
A microservices application is an architectural style where the application is composed of small independent services that communicate
over APIs.

## Traditional vs Vertualization vs Containerization
Traditional :-
Traditional deployment is a manual process where code is deployed to production by a team or individual.

It means :-
1. Developers write code.
2. Give it to operations team.
3. Teams manually installs , configures and deployed it on servers.

Virtualization :-
Virtualization is a technology that allows you to create multiple virtual computers (VMs) on a single physical computer.

Containerazation :-
Containerazation is a technology used in devops to package an application along with all its dependencies (libraries ,framework ,configs) into a single
unit called a  container so it can run anywhere without issues.

## What is Docker?
Docker is an open source platform that automates the deployment of application in containers.


## Installation of Docker
sudo apt update
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker
sudo systemctl status docker
docker --version


## Docker Commands

```shell
docker run [ContainerImage]     # to run a container
docker run -d [ContainerImage]  # to run a container in detached mode
docker ps               # to list running containers
docker ps -a             # to list all containers
docker create [ContainerImage]  # to create a container
docker start [ContainerID]     # to start a container
docker stop [ContainerID]      # to stop a container
docker rm [ContainerID]        # to remove a container]
docker rm -f [ContainerID]     # to force remove a container
docker run -p [HostPort]:[ContainerPort] [ContainerImage]  # to expose a port
docker exec -it [ContainerID] bash  # to attach / access to a container
docker run -P [ContainerImage]  # to expose all ports on random ports from 32768 to 61000
docker logs [ContainerID]   # to check container logs
docker stats [ContainerID]  # to check container resources
```
