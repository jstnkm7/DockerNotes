/var/lib/docker
   aufs
   containers
   images
   volumes

`docker volume create data_volume`

mount the docker to a directory during run command

`docker run -v data_volume:/var/lib/mysql sql`

`docker run -v /data/mysql:/var/lib/mysql sql`

What location are the files related to the docker containers and images stored?

/var/lib/docker

