## Process
**process status**
docker ps
**remove all processes (all,quiet)**
docker rm $(docker ps -aq)
**remove dead processes (all,quiet,filter)**
docker rm $(docker ps -aqf status=exited)

## Pull
**pull down an image**
docker pull [IMG_NAME]

## Run
**pull (if not local) and run an image**
docker run [IMG_NAME]

