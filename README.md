# CI/CD Pipeline Project

## Overview
This project demonstrates an end-to-end CI/CD pipeline using GitHub Actions, Jenkins, and Docker.

## Architecture
- GitHub for source control
- GitHub Actions for CI trigger
- Jenkins for orchestration
- Docker for containerization
- DockerHub for image registry

## Pipeline Flow
1. Developer pushes code
2. GitHub webhook triggers pipeline
3. Jenkins starts build
4. Docker image is created
5. Image pushed to DockerHub
6. Application deployed

## Tech Stack
- GitHub Actions
- Jenkins
- Docker
- Linux
- GitHub Webhooks

## Future Enhancements
- Kubernetes deployment
- Helm charts
- Monitoring with Grafana
- ArgoCD GitOps
