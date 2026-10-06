# Node.js CI/CD using GitHub Actions, Docker & AWS EC2

This project demonstrates deploying a Node.js application using **GitHub Actions, Docker, Docker Compose, GitHub, and AWS EC2**.

## 🛠️ Technologies Used

- Node.js
- Docker
- Docker Compose
- Git & GitHub
- GitHub Actions
- AWS EC2

## 🚀 What I Did

- Launched and configured an **AWS EC2 Ubuntu instance**
- Created a **Node.js application**
- Created a `Dockerfile` and built the Docker image
- Ran the Node.js application inside a **Docker container**
- Created a `docker-compose.yml` file and ran the application using Docker Compose
- Created a GitHub repository and pushed the project using Git
- Cloned the repository on the EC2 instance
- Tested manual deployment using `git pull` and `docker compose up -d --build`
- Created a **GitHub Actions workflow** for deployment
- Configured GitHub Actions to connect to the EC2 server using **SSH**
- Automated the process of:
  - Pulling the latest code
  - Building the Docker image
  - Restarting the application using Docker Compose
- Tested automatic deployment by making changes and pushing them to the `main` branch

## 🔄 Deployment Flow

```text
GitHub Actions
      ↓
     SSH
      ↓
    Server
      ↓
   git pull
      ↓
Updated Code
      ↓
docker compose up -d --build
      ↓
Docker Image Rebuilt
      ↓
New Container Started
      ↓
Updated Application

```

---

📘 **Read the full step-by-step blog here:**  
[Github-Actions](https://visheshblog.hashnode.dev/day-76-git-and-github)
