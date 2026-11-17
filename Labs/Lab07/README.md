# Lab 07: Docker Containers and Images

**Name:** Areeba Hameed
**Registration number:** 2023-BSCS-015
**GitHub username:** areebahameed936-dot

## Overview
Installed and checked Docker and Docker Compose on my Ubuntu server, then used Docker to run PostgreSQL and NGINX containers, manage containers and images, and save a new NGINX image.

## Tasks
1. **Install Docker and Docker Compose:** checked both versions.
2. **PostgreSQL in Docker:** ran `postgres:9.6` without a password (error), then with `POSTGRES_PASSWORD`, and ran `postgres:10.10` alongside it.
3. **Inspect and manage:** `docker info`, `docker search ubuntu`, compared `docker ps` and `docker ps -a`, then restarted, stopped and removed the 9.6 container and its image.
4. **NGINX on two ports:** `nginx` on 6001 and `nginx:1.30.6` on 6002, opened both welcome pages and viewed the logs.
5. **Work inside a container:** `docker attach`, `docker exec`, `docker diff`, `docker inspect`, then `docker commit` to create `nginx:myimage`.

## Structure
```
Labs/Lab07/
├── README.md
├── Lab7_Solution.pdf
└── screenshots/   (17 required screenshots)
```

The full write-up with all screenshots is in `Lab7_Solution.pdf`.
