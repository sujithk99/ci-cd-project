# 🚀 DevOps CI/CD Pipeline Project

This project demonstrates a complete CI/CD pipeline using:

- GitHub
- GitHub Actions
- Jenkins
- Docker
- Kubernetes

The pipeline automatically builds, tests, containerizes, and deploys the application whenever code is pushed to GitHub.

---

# 📌 Project Architecture

Developer → GitHub → GitHub Actions → Jenkins → Docker → Kubernetes

---

# 🛠 Technologies Used

| Tool | Purpose |
|------|----------|
| GitHub | Source Code Management |
| GitHub Actions | Trigger CI/CD Workflow |
| Jenkins | CI/CD Automation |
| Docker | Containerization |
| Docker Hub | Container Registry |
| Kubernetes | Container Orchestration |
| Minikube | Local Kubernetes Cluster |

---

# 📂 Project Structure

```bash
project/
│
├── .github/
│   └── workflows/
│       └── main.yml
│
├── deployment.yaml
├── service.yaml
├── Dockerfile
├── Jenkinsfile
├── package.json
├── index.js
└── README.md
