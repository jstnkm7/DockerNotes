## 

**I. tags**
example:

`docker run redis:4.0`

**II. -i parameter/option flag**

this is for interactive mode

**III -t option flag**

this stands for psuedo terminal

when we have do -it 

``we are both in interactive mode and psuedo terminal**

**IV. Port mapping**

there are two options available:

**option 1:**

use the IP of the docker container. this ip is an internal IP and only accessible within the docker host

**option 2:**

can use the IP of the docker host

in order for that IP to work, we need to map a free port on the docker host to a port on the docker container

docker run -p < host port > : < container port >

`docker run -p 80:5000 nginx`


**V. Volume mapping**

a created volume : docker container volume

docker run -v /opt/datadir:/var/lib/sql mysql






