# Simple Java Application with Jenkins CI/CD and Docker

## Project Overview

This project is a simple Java application built using Maven. It demonstrates how to automate the build and deployment process using Jenkins and Docker.

The project follows a basic CI/CD workflow where Jenkins builds the application, packages it using Maven, creates a Docker image, and prepares it for deployment.


## Technologies Used

- Java
- Maven
- Jenkins
- Docker
- Git
- GitHub
- Linux


## Project Structure

```
Simple-Java-App/
│── src/
│── Dockerfile
│── Jenkinsfile
│── pom.xml
│── .gitignore
```

---

## Prerequisites

Before running this project, install:

- Java JDK
- Maven
- Docker
- Jenkins
- Git

---

## Clone Repository

git clone https://github.com/devrajesh16/Simple-Java-App.git

## Build the Project

mvn clean package

## Build Docker Image

docker build -t simple-java-app .

## Run Docker Container

docker run -d -p 8080:8080 simple-java-app

## Jenkins Pipeline

The Jenkins pipeline performs the following steps:

1. Pulls source code from GitHub
2. Builds the project using Maven
3. Creates the application package
4. Builds the Docker image
5. Deploys the application


## CI/CD Workflow

```
Developer
     │
     ▼
 GitHub Repository
     │
     ▼
 Jenkins
     │
     ▼
 Maven Build
     │
     ▼
 Docker Image
     │
     ▼
 Application Deployment
```




## Author

Rajesh

Aspiring DevOps Engineer
