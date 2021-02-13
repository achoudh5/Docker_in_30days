container is the running environment for image

### STEP 1(on CLI)

client  docker builds the new image
docker build -t <new-image-name> .

### STEP2

check images on CLI

$docker images

### STEP3

Check running containers on CLI

$docker ps

### STEP4

Check all containers evenif not running on CLI

$docker ps -a

### STEP 5

builds the docker image with whatever we specified in dockerfile

$docker build -t myflaskapp .

### STEP6

bash of docker

$docker run -it -d -p 5000:5000 myflaskapp
$sudo docker exec -it <container-id> bash

### STEP7

Remove the stopped containers
The following command removes any stopped containers, unused volumes and networks, and dangling images:

$docker system prune
