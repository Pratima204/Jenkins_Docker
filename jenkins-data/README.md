# ssh-keygen -f remote_key (inside Centos7 dir)
# Run docker -compose up -d inside jenkins-data directory

### To remote all containers
```sh
docker kill $(docker ps -a | cut -d ' ' -f 1)
```

### To remove all images
```sh
docker rmi $(docker images) --force
```
