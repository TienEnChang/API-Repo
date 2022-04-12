# Guide

Preparation
```
sudo apt update
sudo apt upgrade
```
Install Screen & Git
```
sudo apt install screen git
```
Install Docker
```
sudo apt install ca-certificates curl gnupg lsb-release
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
  
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io
sudo docker run hello-world
```
Git Clone
```
git clone https://github.com/TienEnChang/API-Repo.git
```
Docker Pull
```
sudo docker pull strapi/strapi
```
Setup
```
cd API-Repo
docker run -it -p 1337:1337 -v `pwd`:/srv/app strapi/strapi
```

\
[![strapi](https://i.imgur.com/fP5frDe.png)](http://34.82.135.45:1337/admin/)
[![gcloud](https://i.imgur.com/xW6xKYK.png)](https://console.cloud.google.com/compute/instances?hl=zh-TW&project=workspace-328311)
[![dockerhub](https://i.imgur.com/MoWgJSc.png)](https://hub.docker.com/)
