# 🚀 CI/CD Pipeline with GitHub Actions & Docker (Local Deployment)

This project demonstrates a complete CI/CD pipeline using **GitHub Actions**, **Docker**, and **Docker Hub**, deploying a Node.js web application locally via **Minikube** or **Docker CLI** (no cloud services used).

---


---

## ⚙️ Technologies Used

- **GitHub Actions** – CI/CD pipeline automation
- **Docker** – Containerization
- **Docker Hub** – Container image registry
- **Node.js** – Sample application
- **PowerShell / Minikube** – Local deployment environment

---

## 🔄 CI/CD Workflow Summary

Every push to the `main` branch triggers the following steps:

1. ✅ **Checkout the source code**
2. 🧪 (Optional) Run unit tests
3. 🛠️ Build the Docker image
4. 🚀 Push the image to Docker Hub (`mayuresh23/ci-cd-app`)
5. 🧾 CI logs and results shown in GitHub Actions tab

---

## 📦 Docker Image

The Docker image is automatically pushed to:

🔗 [https://hub.docker.com/r/mayuresh23/ci-cd-app](https://hub.docker.com/r/mayuresh23/ci-cd-app)

To pull and run:

```bash
docker pull mayuresh23/ci-cd-app
docker run -d -p 3000:3000 mayuresh23/ci-cd-app


