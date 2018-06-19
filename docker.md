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
docker build -t [MY_IMG] .

## Run
**run, leave container running, enable bash, aui(iactive, TTY, detach)** <br>
docker run -itd [IMG_NAME] bash

**run container that will remove itself if killed** <br>
docker run -itd --rm [IMG_NAME] bash

**run,auto-remove,name** <br>
docker run -itd --rm --name [MY_CONTAINER] [IMG_NAME]

## Enter
**enter a running container as bash** <br>
docker exec -it [CONTAINER] bash

## Stop
docker stop [CONTAINER]
