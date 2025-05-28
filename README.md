# 🚀 DevOps CI/CD Demo Project

This project demonstrates a CI/CD pipeline using Jenkins, Docker, and AWS EC2.

---

## 📁 Project Folder Structure

```
devops-ci-cd-demo/
│
├── app/
│   └── index.html                # Simple web app
├── Dockerfile                   # Containerize the app
├── deploy.sh                    # (Optional) Deployment script
├── Jenkinsfile                  # Jenkins pipeline script
└── README.md                    # Project documentation
```

---

## ⚙ Tools Used

- Jenkins – CI server to automate the pipeline  
- Docker – To build and run containerized app  
- GitHub – Version control and code repository  
- AWS EC2 (Amazon Linux 2) – Hosting Jenkins and Docker  

---

## 🔧 How It Works

1. Developer pushes code to GitHub  
2. Jenkins pipeline triggers on push  
3. Jenkins pulls the latest code  
4. Builds Docker image using Dockerfile  
5. Runs the container on EC2  
6. App is accessible via EC2 Public IP  

---

## 🌐 Result

Access your web app:
