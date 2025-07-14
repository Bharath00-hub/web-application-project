# web-application-project 

A containerized Java-based web application enhanced from [manjukolkar/web-application](https://github.com/manjukolkar/web-application), with CI/CD pipeline automation using Jenkins and deployment-ready Docker support.

##  Project Overview

This project demonstrates the setup and deployment of a Java-based web application using **Maven**, **Docker**, and **Jenkins CI/CD pipeline**. The project is structured for scalable deployment and DevOps workflow automation.

---

##  Key Features

- Java-based web application using Maven (`pom.xml`)
- Docker support for consistent deployment
- CI/CD automation with Jenkins (`Jenkinsfile`)
- Modular project layout with separate `server` and `webapp` components
- Script (`Dockertagupdate.sh`) for dynamic Docker tagging

---

## Tech Stack

| Category        | Tools / Technologies          |
|-----------------|-------------------------------|
| Language        | Java                          |
| Build Tool      | Maven (`pom.xml`)             |
| Containerization| Docker                        |
| CI/CD           | Jenkins, Shell Script         |
| VCS             | Git, GitHub                   |

---

## Project Structure
web-application-project/
├── server/ # Backend Java server logic
├── webapp/ # Frontend files or static content
├── Dockerfile # Docker build file
├── Dockertagupdate.sh # Script for updating Docker tags
├── Jenkinsfile # Jenkins pipeline script
├── pom.xml # Maven project config
└── README.md # Project documentation

2. Build with Maven

mvn clean install

3. Build Docker Image

docker build -t web-application:latest .

4. Run Docker Container

docker run -d -p 8080:8080 web-application:latest
Access your app at: http://localhost:8080

Jenkins CI/CD Pipeline
Connect your Jenkins server to the GitHub repo

Create a Pipeline project and use the provided Jenkinsfile

Configure Docker in Jenkins environment

Use Dockertagupdate.sh to dynamically tag Docker images during build


