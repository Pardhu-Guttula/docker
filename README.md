## Installation
Follow the [official Docker installation guide](https://docs.docker.com/get-docker/) based on your operating system.
---

## Daily Docker Commands
### Basic Commands
```bash
docker version
```
- Show Docker version and information

```bash
docker info
```
-  Display system-wide information
---

### Container Management

#### Create a Container
```bash
docker create -it --name my_container ubuntu:latest bash
```
- Creates a new container named "my_container" based on the latest Ubuntu image and starts an interactive bash session.

```bash
### Create and Start a Container
docker run -it --name new_container nginx:latest
- Creates and starts a new container named "new_container" based on the latest NGINX image.

### List Running Containers
docker ps
- Displays a list of currently running containers.

### List All Containers
docker ps -a
- Shows a list of all containers, including stopped ones.

### Start a Container
docker start my_container
- Starts the "my_container" container.

### Stop a Running Container
docker stop my_container
- Stops the "my_container" container.

### Remove a Container
docker rm my_container
- Removes the "my_container" container.

### Remove a Container Forcefully
docker rm -f my_container
- Removes the "my_container" container.

### Inspect a Container
docker inspect my_container
- Retrieves detailed information about the "my_container" container.

### Fetch the Logs of a Container
docker logs my_container
- Retrieves and displays the logs of the "my_container" container.

### Run a Command in a Running Container
docker exec -it my_container ls /app
- Executes the "ls /app" command in the running "my_container" container.

# Pause all processes within a container
docker pause CONTAINER

# Unpause a paused container
docker unpause CONTAINER

### Kill a Running Container
docker kill my_container
- Forcefully terminates the "my_container" container.

### Restart a Container
docker restart my_container
- Restarts the "my_container" container.
```
---
### Image Management
```bash
# List all images
docker images

# Pull an image from a registry
docker pull IMAGE_NAME[:TAG]

# Build an image from a Dockerfile
docker build [OPTIONS] PATH | URL | -

# Remove one or more images
docker rmi [OPTIONS] IMAGE

# Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
docker tag SOURCE_IMAGE[:TAG] TARGET_IMAGE[:TAG]

# Push an image to a registry
docker push IMAGE_NAME[:TAG]
```
---

### Networks
```bash
# List all networks
docker network ls

# Create a network
docker network create [OPTIONS] NETWORK

# Display detailed information about a network
docker network inspect NETWORK
```
---

### Volumes
```bash
# List all volumes
docker volume ls

# Create a volume
docker volume create [OPTIONS] [VOLUME]

# Display detailed information about a volume
docker volume inspect VOLUME
```
---

### Docker Compose
```bash
# Build and start containers
docker-compose up [OPTIONS]

# Stop and remove containers, networks, and volumes
docker-compose down [OPTIONS]

# List containers
docker-compose ps
```
---

### Miscellaneous
```bash
# Remove all unused containers, networks, and images
docker system prune [OPTIONS]
```