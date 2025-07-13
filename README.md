# Streamlit app Docker Image

## 1. Login with your AWS console and launch an EC2 instance
## 2. Run the following commands

Note: Do the port mapping to this port:- 8501

```bash
sudo apt-get update -y

sudo apt-get upgrade

#Install Docker

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

docker --version


```

```bash
git clone "your-project"

ls

cd [name of your instance]/   # cd st-deploy-demo/

ls


```

```bash
docker build -t sulaymanaziz/stapp1:latest . 
```

```bash
docker images -a  
```

```bash
docker run -d -p 8501:8501 sulaymanaziz/stapp1 
```

```bash
docker ps  
```

```bash
docker stop container_id
```

```bash
docker rm $(docker ps -a -q)
```

```bash
docker login 
```

```bash
docker push sulaymanaziz/stapp1:latest 
```

```bash
docker rmi sulaymanaziz/stapp1:latest
```

```bash
docker pull sulaymanaziz/stapp1
```






