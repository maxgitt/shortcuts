## Process <br>
**process status** <br>
docker ps

**remove all processes (all,quiet)**
docker rm $(docker ps -aq)

**remove dead processes (all,quiet,filter)**
docker rm $(docker ps -aqf status=exited)

## Pull
**pull down an image** <br>
docker pull [IMG_NAME] <br>

## Run
**pull (if not local) and run an image** <br>
docker run [IMG_NAME] <br>

