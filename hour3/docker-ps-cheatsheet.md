
# The `docker ps` command

## List of docker ps command

## To show all containers use the given command:

```
docker ps -a
```

## To show the latest created container (includes all states) 

```
docker ps -l
```

## To show n last created containers (includes all states)

```
docker ps -n=-1
```

## To display total file sizes
```
docker ps -s
```

```
docker container ls
```

## Is Used to list all the running containers.

```
docker container ls -a
```

Is used to list all the containers created irrespective of its state. Here Container is the management command.

## To list all running and stopped containers

```
docker ps -a
```

## To list all running containers (just stating the obvious and also example use of -f filtering option)

```
docker ps -a -f status=running
```

## To list all running and stopped containers, showing only their container id

```
docker ps -aq
```


## To list all running and stopped containers

docker ps -a

## To list all running containers (just stating the obvious and also example use of -f filtering option)

docker ps -a -f status=running

## To list all running and stopped containers, showing only their container id

```
docker ps -aq
```

## To remove all containers that are NOT running

```
docker rm `docker ps -aq -f status=exited`
```

## Show the size of running containers only.

```
docker ps -s
```

## To check the size of all containers use :

```
docker ps -as
```


## To list only the containers SHA1:

```
docker ps -aq --no-trunc
```



## List only the name of all containers (since docker ps list only their names with other information):

```
docker inspect --format='{{.Name}}' $(sudo docker ps -aq --no-trunc)
```
