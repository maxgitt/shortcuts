## Process
**process status** <br>
docker ps

**remove all processes (all,quiet)** <br>
docker rm $(docker ps -aq)

**remove dead processes (all,quiet,filter)** <br>
docker rm $(docker ps -aqf status=exited)

## Pull
**pull down an image** <br>
docker pull [IMG_NAME]

## Run
**pull (if not local) and run an image** <br>
docker run [IMG_NAME]

**run and enter container as bash (interactive, TTY)**
docker run -it [IMG_NAME] bash

**run and leave container running (interative, TTY, detach)** 
docker run -itd [IMG_NAME]

**run a container that will remove itself if killed**
docker

## Enter
**enter a running container as bash**
docker exec -it [CONTAINER] bash
