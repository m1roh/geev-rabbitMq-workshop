# Geev RabbitMQ Workshop

This workshop is open to **everybody** *(even if you are not a developer)*

Follow this step-by-step guide to install and run the tools needed for the workshop, if you are not confident or do not want to install software that you will not reuse, team up with a developer.

## Useful links

**VS Code Install Link** : [VS Code](https://code.visualstudio.com/docs/?dv=osx)

**Node Js Download Link** : [Node Js](https://nodejs.org/dist/v12.14.1/node-v12.14.1.pkg)

**Docker Install Guide** : [Docker](https://docs.docker.com/docker-for-mac/install/)

**Rabbit MQ Tutorials** : [RabbitMQ](https://www.rabbitmq.com/getstarted.html)

## Setup environment

- Install VS Code, Node Js and Docker *(see useful links)*

- Install Git
    - Open a terminal
    - Run 
    ```shell
    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    ```
   *(this will install [Brew](https://brew.sh/index_fr))*
    - Run `brew install git`

- Open a terminal and run 
```shell
docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3-management
```
*(this will run RabbitMQ in a Docker container [More informations](https://registry.hub.docker.com/_/rabbitmq/))*
  
### 1.Direct exchange

- Switch to branch **direct** `git checkout direct`

- Run `npm install` in each sub-directory

### 2.PubSub exchange

- Switch to branch **pubsub** `git checkout pubsub`

### 3.Routing exchange

- Switch to branch **routing** `git checkout routing`

- Run `npm install` in each new sub-directories
