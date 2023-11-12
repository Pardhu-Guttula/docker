## Installation
Follow the [official Docker installation guide](https://docs.docker.com/get-docker/) based on your operating system.
---

## Daily Docker Commands

### Basic Commands
```bash
# Show Docker version and information
docker version

# Display system-wide information
docker info
```
---

### Container Management
```bash
# List running containers
docker ps

# List all containers (running and stopped)
docker ps -a

# Create and start a container
docker run [OPTIONS] IMAGE [COMMAND] [ARG...]

# Start a stopped container
docker start [OPTIONS] CONTAINER

# Stop a running container
docker stop [OPTIONS] CONTAINER

# Restart a container
docker restart [OPTIONS] CONTAINER

# Run a command in a running container
docker exec [OPTIONS] CONTAINER COMMAND [ARG...]

# Fetch the logs of a container
docker logs [OPTIONS] CONTAINER

# Remove one or more containers
docker rm [OPTIONS] CONTAINER

# Kill a running container
docker kill [OPTIONS] CONTAINER

# Pause all processes within a container
docker pause CONTAINER

# Unpause a paused container
docker unpause CONTAINER
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
---

Replace placeholders with actual values. Refer to the [official Docker documentation](https://docs.docker.com/) for detailed usage.
```