# DevOps-Assignment-1
Please complete your DevOps prerequisite course from Kode Kloud and complete your assignment.

### HERE IS THE LINK OF REPO: https://github.com/asadrazatkxel/snap-shot-reactjs-app
---
## Jenkins, Docker, SonarQube CI/CD Pipeline

### Overview
This repository contains my submission for the DevOps prerequisite assignment as part of my onboarding at Tkxel. The goal was to set up a simple CI/CD pipeline using Jenkins, Docker, and SonarQube to perform static code analysis and build Docker images.

## Steps Followed

### 1. Create GitHub Repository
- I created a public GitHub repository named `snap-shot-reactjs-app` to host my project.
- A sample ReactJS project was committed to the `main` branch, with additional branches for development (`dev` branch).

### 2. Install Docker on Local Machine
- I used a Linux Bash script to install Docker on my local machine. The script included:
  - Installing Docker from the official Docker repository.
  - Managing Docker service to ensure it starts on boot.
  - Reading about Docker fundamentals like volumes, networks, and container management.

### 3. Set Up Jenkins and SonarQube Using Docker-Compose
- A `docker-compose.yml` file was created to spin up both Jenkins and SonarQube containers. This allowed me to manage both tools locally.
  - **Jenkins:** Used to manage CI/CD pipelines.
  - **SonarQube:** Integrated for code quality and security analysis.

### 4. Create Jenkins Declarative Pipeline
- A Jenkins declarative pipeline was written with the following stages:
  1. **Checkout Code:** Pull code from the `dev` branch of the GitHub repository.
  2. **SonarQube Analysis:** Perform static code analysis using SonarQube.
  3. **Docker Build:** Build a Docker image of the application.

### 5. Commit Bash Script and Docker-Compose File
- Both the Bash script for Docker installation and the `docker-compose.yml` file for Jenkins and SonarQube containers were committed to the repository for reference.

## Challenges Faced
- **SonarQube Integration:** Configuring SonarQube took some time due to authentication and tool configuration issues. I had to ensure proper SonarQube server and scanner configuration in Jenkins.
- **Pipeline Errors:** Initially, I encountered errors while running the Jenkins pipeline due to incorrect tool setup (SonarScanner), which was resolved by configuring Jenkins Global Tool properly.
- **Network Issues:** Running both Jenkins and SonarQube in Docker required some learning about Docker networking, especially when linking containers together.

## What I Learned
- **Docker Basics:** I deepened my understanding of Docker, including how to create volumes, networks, and manage services.
- **CI/CD Pipelines:** Setting up a complete CI/CD pipeline with Jenkins and SonarQube allowed me to explore how modern DevOps tools can automate the software lifecycle.
- **Problem Solving:** The challenges I faced during tool setup (e.g., SonarQube scanner and Docker-compose) taught me how to troubleshoot and resolve integration issues effectively.

## Conclusion
This assignment gave me hands-on experience with essential DevOps practices and tools, helping me understand how continuous integration and delivery pipelines can enhance software development efficiency. I now feel more confident in setting up and managing DevOps environments.
