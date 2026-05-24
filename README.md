# CI/CD Pipeline Project

## Overview

This project demonstrates an end-to-end CI/CD pipeline using GitHub Actions, Jenkins, and Docker.

The pipeline automates:
- Code integration
- Build process
- Docker image creation
- Image publishing to DockerHub
- Automated deployment

The primary goal of this project is to implement a practical DevOps workflow using CI/CD automation and containerization technologies.

---

## Architecture

- GitHub for source control
- GitHub Actions for CI trigger
- Jenkins for orchestration
- Docker for containerization
- DockerHub for image registry
- Linux server for deployment

---

## Architecture Diagram

![CI/CD Architecture](architecture-diagram.png)

---

## Pipeline Flow

1. Developer pushes code to GitHub repository
2. GitHub webhook triggers GitHub Actions
3. GitHub Actions starts CI workflow
4. Jenkins pipeline is triggered
5. Application build process starts
6. Docker image is created
7. Docker image is pushed to DockerHub
8. Deployment server pulls latest Docker image
9. Existing container is replaced with updated container
10. Application becomes available to users

---

## Technologies Used

| Technology | Purpose |
|---|---|
| GitHub | Source Code Management |
| GitHub Actions | Continuous Integration |
| Jenkins | Pipeline Orchestration |
| Docker | Containerization |
| DockerHub | Image Registry |
| Linux | Deployment Environment |

---

## Repository Structure

```text
ci-cd-project/
│
├── .github/
│   └── workflows/
│       └── ci.yml
│
├── app/
│
├── Dockerfile
├── Jenkinsfile
├── docker-compose.yml
├── requirements.txt
├── architecture-diagram.png
└── README.md
```

---

## CI/CD Workflow

### Continuous Integration
- Automatic pipeline trigger on code push
- Source code checkout
- Build validation
- Test execution
- Docker image creation

### Continuous Deployment
- Push Docker image to DockerHub
- Pull latest image on deployment server
- Replace old running container
- Start updated application container

---

## Docker Commands Used

### Build Docker Image

```bash
docker build -t your-image-name .
```

### Run Docker Container

```bash
docker run -d -p 8080:8080 your-image-name
```

### Push Docker Image

```bash
docker push your-dockerhub-username/your-image-name
```

---

## Jenkins Pipeline Stages

- Checkout Code
- Build Application
- Run Tests
- Build Docker Image
- Push Docker Image
- Deploy Application

---

## Future Enhancements

- Kubernetes deployment
- Helm chart integration
- ArgoCD GitOps workflow
- Monitoring using Prometheus and Grafana
- Automated rollback strategy
- Multi-environment deployment
- Security scanning integration

---

## Design Decisions

### Why Docker before Kubernetes?

The project focuses on mastering CI/CD fundamentals and container lifecycle management before moving to orchestration platforms like Kubernetes.

### Why Jenkins with GitHub Actions?

GitHub Actions provides SCM-native automation while Jenkins simulates enterprise-grade pipeline orchestration commonly used in production environments.

---

## Project Objective

This project was designed to demonstrate practical DevOps skills including:
- CI/CD automation
- Containerization
- Pipeline orchestration
- Deployment automation
- Docker image lifecycle management
- Infrastructure workflow understanding

---

## Author

Sujith Kumar S
