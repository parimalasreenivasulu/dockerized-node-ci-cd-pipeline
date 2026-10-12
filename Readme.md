# Containerized Node.js App with PostgreSQL & Redis

[![CI/CD Pipeline](https://github.com/parimalasreenivasulu/dockerized-node-ci-cd-pipeline/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/parimalasreenivasulu/dockerized-node-ci-cd-pipeline/actions)

An end-to-end DevOps project featuring a multi-container Node.js backend connected to PostgreSQL and Redis, fully containerized using Docker and deployed via an automated GitHub Actions CI/CD pipeline.

---

## 🛠️ Tech Stack & Tools

* **Backend:** Node.js, Express.js
* **Databases:** PostgreSQL, Redis
* **Containerization:** Docker, Docker Compose (Multi-stage build)
* **CI/CD Pipeline:** GitHub Actions
* **Version Control:** Git, GitHub

---

## 🚀 CI/CD Pipeline Workflow

The GitHub Actions pipeline (`.github/workflows/ci-cd.yml`) automates quality control and build verification on every push or pull request to the `main` branch:

1. **Linting:** Runs code quality checks (`npm run lint`).
2. **Testing:** Executes automated unit tests (`npm test`).
3. **Docker Build:** Builds multi-stage Docker images with build cache optimizations (`docker/build-push-action`).

---

## 📂 Project Structure

```text
dockerized-node-ci-cd-pipeline/
├── .github/
│   └── workflows/
│       └── ci-cd.yml       # GitHub Actions pipeline workflow
├── Dockerfile              # Multi-stage Docker build configuration
├── docker-compose.yml      # Multi-container orchestration (Node, Postgres, Redis)
├── server.js               # Node.js application entry point
├── package.json            # Dependencies and scripts
└── README.md               # Project documentation
