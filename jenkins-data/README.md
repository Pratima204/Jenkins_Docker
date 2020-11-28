### ssh-keygen -f remote_key (inside Centos7 dir)
### To install docker compose use this command
```sh
sudo curl -L "https://github.com/docker/compose/releases/download/1.27.4/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /user/local/bin/docker-compose 

```
### Run docker-compose up -d inside jenkins-data directory

### To remote all containers
```sh
docker kill $(docker ps -a | cut -d ' ' -f 1 | sed 1d)
```

### To remove all images
```sh
docker rmi $(docker images) --force
```


###  You can use this on userdata for installing docker and git
```sh
#!/bin/bash 
amazon-linux-extras install docker
service docker start
usermod -a -G docker ec2-user
yum install git -y

```





