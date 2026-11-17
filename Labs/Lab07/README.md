##Lab 07: Docker Containers and Images

Name: Areeba Hameed
Registration number: 2023-BSCS-015
GitHub username: areebahameed936-dot

Overview

Installed and checked Docker and Docker Compose on my Ubuntu server, then used Docker to run PostgreSQL and NGINX containers, manage containers and images, and save a new NGINX image.

##Tasks
Install Docker and Docker Compose: checked both versions.
PostgreSQL in Docker: ran postgres:9.6 without a password (error), then with POSTGRES_PASSWORD, and ran postgres:10.10 alongside it.
Inspect and manage: docker info, docker search ubuntu, compared docker ps and docker ps -a, then restarted, stopped and removed the 9.6 container and its image.
NGINX on two ports: nginx on 6001 and nginx:1.30.6 on 6002, opened both welcome pages and viewed the logs.
Work inside a container: docker attach, docker exec, docker diff, docker inspect, then docker commit to create nginx:myimage.

