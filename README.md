<div align="center">

# 🚀 GitHub Actions Docker Pipeline

### Production-ready CI/CD Pipeline using GitHub Actions, Docker & Next.js

![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI/CD-blue?logo=githubactions)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-black?logo=next.js)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

</div>

---

# 📖 Overview

This project demonstrates a **complete production-ready CI/CD pipeline** using **GitHub Actions**, **Docker**, and **Next.js**.

Whenever code is pushed or a new version tag is created, GitHub Actions automatically builds, tests, creates Docker images, pushes them to Docker Hub, and deploys the application.

---

# ✨ Features

- ✅ GitHub Actions CI/CD
- ✅ Docker Image Build
- ✅ Docker Version Tagging
- ✅ Docker Hub Push
- ✅ Automatic Deployment
- ✅ GitHub Secrets
- ✅ Version-based Releases
- ✅ Production-ready Workflow
- ✅ Next.js Application
- ✅ Multiple GitHub Workflows

---

# 🛠 Tech Stack

| Technology | Purpose |
|------------|----------|
| Next.js | Frontend Framework |
| Node.js | Runtime |
| Docker | Containerization |
| GitHub Actions | CI/CD |
| Docker Hub | Image Registry |
| Git | Version Control |

---

# 📁 Project Structure

```text
.
├── .github
│   └── workflows
│       ├── deploy.yml
│       ├── docker.yml
│       └── docker-version.yml
│
├── app/
├── public/
│
├── Dockerfile
├── .dockerignore
├── package.json
├── next.config.ts
├── README.md
└── ...
```

---

# ⚙ CI/CD Workflow

```text
Developer
     │
     ▼
Git Push
     │
     ▼
GitHub Repository
     │
     ▼
GitHub Actions
     │
 ┌───┴──────────────┐
 │                  │
 ▼                  ▼
Build           Run Checks
 │                  │
 └──────────┬───────┘
            ▼
     Docker Build
            │
            ▼
 Push Docker Image
            │
            ▼
 Production Deploy
```

---

# 🏗 Workflow Files

| Workflow | Description |
|----------|-------------|
| docker.yml | Build Docker Image |
| docker-version.yml | Build & Push Version Tags |
| deploy.yml | Deploy Application |

---

# 🐳 Docker

## Build Image

```bash
docker build -t cicd-app .
```

---

## Run Container

```bash
docker run -d -p 3000:3000 cicd-app
```

---

## Stop Container

```bash
docker stop <container_id>
```

---

## Remove Container

```bash
docker rm <container_id>
```

---

# 🚀 Run Locally

Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/github-actions-docker-pipeline.git
```

Move into Project

```bash
cd github-actions-docker-pipeline
```

Install Dependencies

```bash
npm install
```

Start Development Server

```bash
npm run dev
```

Visit

```
http://localhost:3000
```

---

# 🐳 Build Docker Image

```bash
docker build -t cicd-app .
```

Run

```bash
docker run -p 3000:3000 cicd-app
```

---

# 🏷 Version Release

Create Version

```bash
git tag v1.0
```

Push Version

```bash
git push origin v1.0
```

GitHub Actions automatically:

- Detects new version
- Builds Docker Image
- Tags Docker Image
- Pushes Docker Image

---

# 🔐 GitHub Secrets

Required Secrets

```
DOCKER_USERNAME

DOCKER_PASSWORD

SERVER_HOST

SERVER_USER

SERVER_PASSWORD

SERVER_PORT

SSH_PRIVATE_KEY
```

---

# 📦 Docker Image

Example

```
docker pull yourusername/cicd-app:latest

docker pull yourusername/cicd-app:v1.0
```

---

# 📷 CI/CD Flow

```text
Push Code
    │
    ▼
GitHub Actions
    │
    ▼
Install Packages
    │
    ▼
Build Next.js
    │
    ▼
Docker Build
    │
    ▼
Docker Hub
    │
    ▼
Deployment
```

---

# 📌 Future Improvements

- Kubernetes Deployment
- AWS ECS
- GitHub Container Registry
- SonarQube
- Slack Notifications
- Multi-stage Docker Build
- Security Scan
- Automated Testing

---

# 🤝 Contributing

1. Fork Repository

2. Create Branch

```bash
git checkout -b feature/new-feature
```

3. Commit

```bash
git commit -m "Added new feature"
```

4. Push

```bash
git push origin feature/new-feature
```

5. Open Pull Request

---

# 👨‍💻 Author

**Kalana Siyambalapitiya**

GitHub

https://github.com/KalanaSiyambalapitiya

---

# ⭐ Show your support

If you found this project helpful,

⭐ Star this repository

🍴 Fork it

📢 Share it

---

# 📄 License

MIT License

---

<div align="center">

## 🚀 Happy Coding!

Made with ❤️ using GitHub Actions & Docker

</div>This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
