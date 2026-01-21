# Self-Hosted GitLab with GitLab Runner (Docker Compose)

This repository provides a **Docker Compose setup** for running a **self-hosted GitLab CE server** along with a **GitLab Runner** on a local machine or private server.

It is useful for learning GitLab CI/CD, testing pipelines locally, and understanding self-hosted DevOps infrastructure.

---

## 🧱 Architecture Overview

- **GitLab CE**  
  - Hosts repositories
  - Manages users, issues, and CI/CD pipelines
- **GitLab Runner**
  - Executes CI/CD jobs
  - Uses Docker executor
- **Docker Compose**
  - Manages multi-container setup
  - Persistent volumes for data safety

---

## 🛠 Tech Stack

- Docker
- Docker Compose
- GitLab CE (Community Edition)
- GitLab Runner
- Linux-based containers

---

## 📁 Services Included

### 1️⃣ GitLab Server
- Image: `gitlab/gitlab-ce`
- Exposed on port **8000**
- Persistent storage for:
  - Configuration
  - Logs
  - Repository & CI data

### 2️⃣ GitLab Runner
- Image: `gitlab/gitlab-runner`
- Docker executor enabled
- Connected to host Docker daemon
- Ready for CI/CD execution

---

## ⚙️ Prerequisites

- Docker installed
- Docker Compose installed
- Minimum **4 GB RAM** recommended
- Linux / Windows (WSL2 recommended) / macOS

---

## 🚀 Setup & Usage

### Clone the repository
```bash
git clone https://github.com/your-username/self-hosted-gitlab-with-runner.git
cd self-hosted-gitlab-with-runner
