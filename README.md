# DockerContainers

A list of Docker containers to experiment

## Portainer

Container Management tool

https://github.com/portainer/portainer

$ docker run -d -p 9000:9000 portainer/portainer

To run on the same host:

$ docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer

Your Portainer will be running at: http://localhost:9000

## Couchbase

docker run -d --name db -p 8091-8094:8091-8094 -p 11210:11210 couchbase

https://hub.docker.com/_/couchbase/

## Microsoft SQL Server

sudo docker pull microsoft/mssql-server-linux:2017-latest

docker run -e 'ACCEPT_EULA=Y' \
-e 'SA_PASSWORD=Passw0rd!' \
-p 1433:1433 \
--name mssql \
-d microsoft/mssql-server-linux:2017-latest

## Raven DB

docker run -p 8080:8080 ravendb/ravendb

https://hub.docker.com/r/ravendb/ravendb/

Test