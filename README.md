# Containerization-of-Java-App
Containerized Java Application


<a href="https://github.com/hashtagesteban/vprofile-project/tree/containers">Source code and Dockerfiles</a>

## Architecture


## Objectives
### Identify which docker files we must build:
Tomcat - multi-stage dockerfile:
          openjdk:11 to build artifact
          Copy artifact to tomcat 

MYSQL - set env variables
        load database 

NGINX - remove default config file
        add our own config file


### Memcached and RabbitMQ do not need any config changes

Set env variables

### Create Docker Compose file :
Services:
  -app
  -db
  -web
  -cache
  -mq

Volumes:
vproappdata
vprodbdata

### Build and Run docker images


