# INSTALATION - DOCKER, PORTAINER AND NGINX PROXY MANAGER

### Process

1 - Install docker

```
curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo groupadd docker

sudo usermod -aG docker $USER

docker run hello-world
```

2 - Install portainer

```
docker swarm init

curl -L https://downloads.portainer.io/ce2-18/portainer-agent-stack.yml -o portainer-agent-stack.yml

docker stack deploy -c portainer-agent-stack.yml portainer
```

3 - Install Nginx Proxy Manager

Copy the stack available in the repository

https://github.com/IsraelXabregas/docker-npm

Log in with the default NPM user

```
Email:    admin@example.com
Password: changeme
```
