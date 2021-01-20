# Docker
Docker installation and docker file

##########Installing Docker############    
sudo apt-get remove docker docker-engine docker.io containerd runc
sudo apt-get update
sudo apt-get install     apt-transport-https     ca-certificates     curl     gnupg-agent     software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo apt-key fingerprint 0EBFCD88
udo add-apt-repository    "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
sudo apt-get install docker-ce docker-ce-cli containerd.io

List docker which are running
#docker ps

Command to pull image
#docker pull hello-world

List all the images pulled
#docker images

remove Images
#docker rmi bf756fb1ae65

Force remove images
#docker rmi -f bf756fb1ae65

Command to run Docker
#docker run hello-world
#docker ps

List all the container including terminated one
#docker ps -a

Below command checks of the image is locally present els it will pull from hub
#docker run -id ubuntu
#docker ps
#docker run -id ubuntu
#docker ps

Command to login to docker
#docker exec -it 41d4bfa06cb5-->container ID
#docker exec -it 41d4bfa06cb5 "bash"



