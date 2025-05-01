# Node.js Web Application Deployment with Jenkins, Docker, and Kubernetes

## 📌 Project Overview
This project demonstrates the complete DevOps lifecycle for deploying a simple Node.js web application using a CI/CD pipeline. The pipeline uses Jenkins to automate build and deployment, Docker to containerize the application, and Kubernetes (K8s) for scalable deployment on AWS EC2.

---

## 🛠️ Tech Stack
- Node.js
- Jenkins
- Docker
- Kubernetes
- Docker Hub
- AWS EC2
- Git

---

## ⚙️ Pipeline Workflow
1. **Code Push** to Git triggers Jenkins.
2. Jenkins **builds the Docker image** and pushes to Docker Hub.
3. Jenkins deploys to a **Kubernetes Cluster** on AWS EC2.
4. Kubernetes handles **rolling updates** and service exposure.

---

## 📂 Project Structure

nodejs-app/ ├── Dockerfile ├── app.js ├── package.json ├── jenkins/ │ └── Jenkinsfile ├── k8s/ │ ├── deployment.yaml │ └── service.yaml └── README.md


---

## 🚀 Deployment Steps
1. Clone the repo
2. Build the Docker image
```bash
docker build -t firos/nodejs-app .

    Push to Docker Hub

docker push firos/nodejs-app

    Apply Kubernetes manifests

kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml



    Add Jenkins pipeline, Docker Hub image, and running app screenshots.

🙋 About Me

This project was built by Firos as part of hands-on DevOps practice. I am an aspiring Junior DevOps Engineer passionate about automation and cloud infrastructure.

📧 Email: firosop0786@gmail.com
📍 Location: Chennai, India
