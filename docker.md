## Process
**process status**
docker ps

## Run
# pull down an image
docker pull [IMG_NAME]
 
# pull (if not local) and run an image
docker run [IMG_NAME]

##
# remove leftover images
docker rm $(docker ps -aq)
