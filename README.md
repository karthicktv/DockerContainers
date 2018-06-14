# DockerContainers
A list of experimental Docker containers

## Portainer

Container Management tool

https://github.com/portainer/portainer

docker run -d -p 9000:9000 portainer/portainer

To run on the same host:

docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer

Your Portainer will be running at: http://localhost:9000