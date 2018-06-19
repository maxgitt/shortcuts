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

## Build
**build an image and give it a name (tag)** (don't forget the period) <br>
docker build -t [MY_NAME] .

## Run
**pull (if not local) and run an image** <br>
docker run [IMG_NAME]

**run and enter container as bash (interactive, TTY)** <br>
docker run -it [IMG_NAME] bash

**run and leave container running (interative, TTY, detach)** <br>
docker run -itd [IMG_NAME]

**run a container that will remove itself if killed** <br>
docker

## Enter
**enter a running container as bash** <br>
docker exec -it [CONTAINER] bash
