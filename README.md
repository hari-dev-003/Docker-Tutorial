# Docker Tutorial
Docker is a containerization platform that allows developers to package, ship, and run applications in containers

## Why Docker ?
    
- **Portability**: Docker containers can run on any system that has Docker installed, regardless of the underlying operating system.
- **Isolation**: Containers isolate applications from the host system and from each other, ensuring that they don't interfere with each other's operations.
- **Efficiency**: Containers are lightweight and start quickly, making them efficient in terms of resource utilization.
- **Scalability**: Docker makes it easy to scale applications by running multiple instances of containers across a cluster of machines.

## Docker Container

 - It is a single unit that consists of our application packed with dependencies.
 - As the dependencies are packed with containers they are independent on platform for running.
  - Containers are portable i.e sharable 
   - Lightweight in Nature
   - Using containers we can build apps with various dependencies in a single machine

## Docker Image
  &nbsp; &nbsp; It is a executable file which contains instructions to build docker containers

  ``` 
____________________________________
|                                   |
|         Operating System          |
|  _______________________________  |
|  |                              | |
|  |                              | |
|  |        Docker Image          | |
|  |                              | |
|  | _____________________________| |
|  |                              | |
|  |    Docker Container          | |
|  |_____________________________ | |
|                                   |
|___________________________________|


  ````

## Docker Commands


**Docker pull** - Pull an image from a registry
```
docker pull <image_name>
```

**Docker images** - Lists images in our account
```
docker images
```

**Docker run** - Creates a container of the image and Runs it

 - **flags**
    - **-d**: Detached mode: Run container in background
    - **-p**: Port mapping: Maps a container port to a host port
    - **-v**: Volume mapping: Maps a container directory to a host directory
    - **-it**: Interactive mode: Allocates a pseudo-TTY and keeps STDIN open ev

```
docker run <image_name>
```

**Docker ps** - Lists the Containers that is running currently

 - **flags**
    - **-a**: Show all containers (including stopped ones)
    - **-f**: Filter output based on conditions
    - **-q**: Only display container IDs
    - **-l**: Show the latest created container
    - **-n**: Show the number of containers that are running
    - **-s**: Show the size of the container

**Docker start** - Starts the Specified container
```
docker start <container_id> or <container_name>

```
**Docker stop** - Stops the running container 

```
docker stop <container_id> or <container_name>
```
**Docker rm** - Removes the container
```
docker rm <container_id> or <container_name>
```
**Docker rmi** - Removes the existing image 
```
docker rmi <image_id> or <image_name>
```
**Docker exec** - Runs a command in a running container
```
docker exec -it <container_id> <command>
```
