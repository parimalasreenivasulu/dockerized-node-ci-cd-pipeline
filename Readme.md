# Containerized Node.js App with PostgreSQL & Redis

A production-ready, multi-stage containerized Node.js application built with Express, PostgreSQL, and Redis, orchestrated using Docker Compose. Developed with a strong focus on security, lightweight footprints, and best practices.

## 🚀 Tech Stack
* **Runtime:** Node.js (Alpine Linux)
* **Web Framework:** Express.js
* **Database:** PostgreSQL (Alpine)
* **Cache:** Redis (Alpine)
* **Containerization:** Docker & Docker Compose (Multi-stage builds)

## ✨ Key Features
* **Multi-Stage Docker Build:** Separates build-time dependencies from the production runtime environment to drastically reduce image size.
* **Security Hardened:** Runs under a dedicated non-root user (`nodejs`) instead of root to minimize potential container security vulnerabilities.
* **Service Orchestration:** Automated startup sequence using Docker Compose with built-in health checks for the PostgreSQL database.
* **Persistent Storage:** Configured with Docker volumes to ensure data persistence for both PostgreSQL and Redis.

## 🛠️ Prerequisites
Make sure you have the following installed on your machine:
* [Docker Desktop](https://www.docker.com/products/docker-desktop/)

## 🏃‍♂️ How to Run Locally

1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git)
   cd YOUR-REPO-NAME