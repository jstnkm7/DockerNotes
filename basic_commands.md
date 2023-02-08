## Docker Command List
---
Get docker containers on host:  

  - `docker ps`
  
Get all docker containers including stopped/exited containers:

- `docker ps -a` 
  

- `docker images`

- `docker run <docker/image-name>`

I. Deleting Containers

Deleting containers one-by-one:

- `docker stop <container id | container name>`

- `docker rm <container id | container name>`

To stop all the containers at once, run the command:
- `docker stop $(docker ps -aq)`

- To remove all the stopped containers at once, run the command: 

   `docker rm $(docker ps -aq)`

II. Deleting images

- `docker rmi <image-name>`
  
  Deleting all the docker images at once

- `docker rmi $(docker images -aq)`