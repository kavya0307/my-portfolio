# 🌐 Portfolio Website - Dockerized Deployment with Nginx Reverse Proxy

A personal portfolio website showcasing my projects, technical skills, certifications, and achievements. This project demonstrates modern cloud deployment practices by hosting a Dockerized web application on an AWS EC2 instance with Nginx configured as a reverse proxy.

---

# 🚀 Live Demo

### AWS EC2 + Docker + Nginx

http://YOUR-EC2-PUBLIC-IP

---

# 🛠 Technologies Used

- HTML5
- CSS3
- Docker
- Nginx
- Git
- GitHub
- GitHub Actions
- Docker Hub
- AWS EC2
- Linux (Ubuntu)

---

# ✨ Features

- Responsive portfolio website
- Dockerized web application
- Hosted on AWS EC2
- Nginx Reverse Proxy configuration
- Automated Docker image build using GitHub Actions
- Docker Hub integration
- Cloud-based deployment
- Linux server management
- SSH-based server access

---

# 📂 Project Structure

```
portfolio/
│
├── .github/
│   └── workflows/
│       └── docker.yml
│
├── images/
├── index.html
├── style.css
├── Dockerfile
├── README.md
└── assets/
```

---

# ☁️ Project Deployment Workflow

```
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
      ▼
Build Docker Image
      │
      ▼
Push Image to Docker Hub
      │
      ▼
AWS EC2 Instance
      │
      ▼
Docker Container
      │
      ▼
Nginx Reverse Proxy
      │
      ▼
Portfolio Website
```

---

# 🐳 Docker Deployment

- Created a Dockerfile for the portfolio website
- Built the Docker image
- Executed the application inside a Docker container
- Exposed the container using port mapping
- Verified application deployment inside the EC2 instance

Example:

```
docker build -t portfolio-website .

docker run -d -p 8080:80 --name portfolio-container portfolio-website
```

---

# 🌐 Nginx Reverse Proxy

Configured Nginx to act as a reverse proxy between the client and the Docker container.

Workflow:

```
Internet
      │
      ▼
Nginx (Port 80)
      │
      ▼
Docker Container (Port 8080)
      │
      ▼
Portfolio Website
```

Benefits:

- Routes incoming HTTP requests
- Improves security
- Simplifies application access
- Supports future scalability

---

# 🔐 Secure Deployment

Implemented secure deployment practices by using:

- SSH key-based authentication
- GitHub Secrets
- Docker Hub Access Token

Sensitive credentials are securely stored in GitHub Secrets and are never exposed in the repository.

---

# ⚙️ CI/CD Pipeline

Implemented Continuous Integration using GitHub Actions.

Pipeline Flow:

```
Code Changes
      │
      ▼
Git Push
      │
      ▼
GitHub Actions
      │
      ▼
Build Docker Image
      │
      ▼
Push Docker Image to Docker Hub
```

---

# 📚 Learning Outcomes

Through this project, I gained practical experience in:

- Docker Containerization
- Linux Server Administration
- AWS EC2
- Nginx Reverse Proxy
- Port Mapping
- SSH Authentication
- GitHub Actions
- CI/CD Automation
- Docker Hub
- Cloud Deployment
- DevOps Fundamentals

---

# 🎯 Key Concepts Learned

- Difference between Public Port and Container Port
- Reverse Proxy Architecture
- Docker Image and Container Lifecycle
- Linux Server Configuration
- SSH Key Authentication
- GitHub Secrets
- Automated Deployment Workflow
- Cloud-based Application Hosting

---

# 📖 Future Enhancements

- Configure HTTPS using SSL/TLS
- Deploy using a custom domain
- Implement Continuous Deployment (CD)
- Add monitoring and logging
- Container orchestration using Kubernetes

---

# 👩‍💻 Author

**Kaviya Sri**

B.Tech - Artificial Intelligence and Machine Learning

GitHub:
https://github.com/kavya0307

LinkedIn:
https://www.linkedin.com/in/kavyasri1503