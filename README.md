# Docker Command
## For only me
-----------------

## Check docker version
```
  docker -v
```

## Download docker images
```
  docker pull {Image-name}:{tag}
  # EX: docker pull python:3 
  # tag is not necessary
```

## Show what images are in the local
```
  docker images
```

## Create container using image
```
  docker create {Option} {Image-name}:{tag}
  # EX: docker create -it python
```

## Start container
```
  docker start {Container ID or Name}
```

## Use CLI of each container
```
  docker attach {Container ID or Name}
```

## When Image is not in the local, download Image and run directly.
```
  docker run {Image-name}:{tag}
  # EX: docker -it run python:3
```

## Restart container which is running now
```
  docker restart {Container ID or Name}
```

## Get out from interner shell of container
```
  exit
```

## Show container which is running now
```
  docker ps
```

## Show all containers
```
  docker ps -a
```

## Delete container
```
  docker rm {Container ID or Name}
```

## Delete all containers
```
  docker rm `docker ps -a -q`
```

## Delete image
```
  docker rmi {Option} {Image ID}
  
  -f Option can delete image even if there is container
```

## Stop all containers
```
  docker stop $(docker ps -aq)
```

## Delete all docker elements(Container, Image, Network, Volume....) which is not using.
```
  docker system prune -a
```

## Make image using dockerfile
```
  # Basedir is folder directory which has Dockerfile  
  # . at the last is relative path
  docker build -t {Image-name} .
```

## Run docker compose
```
  docker-compose up
```
