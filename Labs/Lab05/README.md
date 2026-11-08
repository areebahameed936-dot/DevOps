# Lab 05: Build, Test, and Package Applications with IntelliJ IDEA and Docker

**Name:** Areeba Hameed
**Registration number:** (2023-BSCS-25)
**Section:** A
**GitHub username:** areebahameed936-dot

## Overview

In this lab I launched IntelliJ IDEA through a Docker-based browser desktop, cloned four sample projects, and built, tested, packaged and ran them. I also built a Docker image from an existing Dockerfile.

## Tasks

| Task | Description | Key result |
|------|-------------|------------|
| 1 | Clone `Intellij-Idea-docker`, run `setup.sh`, open IntelliJ at `https://localhost:3001` | IntelliJ running in the browser desktop |
| 2 | Maven project (`java-maven-app`): install Maven, add Elasticsearch 7.0.0, `mvn package`, `mvn test`, run the JAR | `target/java-maven-app-1.1.0-SNAPSHOT.jar` |
| 3 | Gradle project (`java-app`): use JDK 16, add Elasticsearch 7.0.0, `./gradlew build`, run the JAR | `build/libs/java-app-1.0-SNAPSHOT.jar` |
| 4 | Node.js project (`node-project`): `npm install`, `npm start` (port changed to 4000), `npm test`, `npm pack` | `bootcamp-node-project-1.0.0.tgz` |
| 5 | React/Node API (`react-nodejs-example`): `npm install`, `npm run build` (webpack) | `api/server.bundle.js` |
| 6 | Build a Docker image from the Node.js project's Dockerfile | `lab5:1.0` |

## Main Commands

```bash
# Task 1 (host terminal)
git clone https://github.com/WaqasSaleem97/Intellij-Idea-docker.git
cd Intellij-Idea-docker && bash setup.sh && docker compose ps

# Task 2 (IntelliJ terminal)
sudo apt install -y maven && mvn --version
mvn package && mvn test
java -jar target/java-maven-app-1.1.0-SNAPSHOT.jar

# Task 3
./gradlew --version && ./gradlew build
java -jar build/libs/java-app-1.0-SNAPSHOT.jar

# Task 4
sudo apt install -y nodejs npm
cd app && npm install && npm start && npm test && npm pack

# Task 5
cd api && npm install && npm run build

# Task 6
sudo docker images
sudo docker build -t lab5:1.0 .
sudo docker images
```

## Folder Structure

```
Labs/
└── Lab05/
    ├── README.md
    ├── Lab5_Solution.pdf
    └── screenshots/    (37 screenshots)
```

## Submission

The full `Labs/Lab05` directory (README, `Lab5_Solution.pdf` and `screenshots/`) is committed and pushed to the `DevOps` repository.
