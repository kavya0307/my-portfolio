# AWS S3 + CloudFront Portfolio Website | Docker & EC2 Deployment

## Objective

Host a static portfolio website using AWS S3 and CloudFront, then containerize and deploy the application using Docker on an AWS EC2 instance.

## Technologies Used

* HTML
* CSS
* Git
* GitHub
* AWS S3
* AWS CloudFront
* Docker
* AWS EC2
* Ubuntu Linux

## Features

* Responsive Portfolio
* Hero Section
* About Section
* Project Cards
* Contact Section
* HTTPS Delivery via CloudFront
* Docker Containerization
* Cloud Deployment using AWS EC2
* Public Access via EC2 Instance

## Task 1: S3 + CloudFront Deployment

### Deployment Steps

1. Created portfolio website using HTML/CSS.
2. Uploaded source code to GitHub.
3. Hosted website on AWS S3.
4. Configured CloudFront for HTTPS delivery.

## Task 2: Docker + EC2 Deployment

### Deployment Steps

1. Installed Docker Desktop on Windows.
2. Created a Dockerfile for the portfolio website.
3. Built a Docker image using Nginx.
4. Ran the website locally in a Docker container.
5. Created an Ubuntu EC2 instance on AWS.
6. Installed Docker on the EC2 server.
7. Cloned the GitHub repository to EC2.
8. Built the Docker image on EC2.
9. Ran the Docker container on EC2.
10. Accessed the portfolio website through the EC2 public IP.

## Docker Commands Used

### Build Docker Image

```bash
docker build -t portfolio-website .
```

### Run Docker Container

```bash
docker run -d -p 8080:80 --name portfolio-container portfolio-website
```

### List Images

```bash
docker images
```

### List Running Containers

```bash
docker ps
```

## EC2 Deployment Commands

### Update Ubuntu

```bash
sudo apt update
```

### Install Docker

```bash
sudo apt install docker.io -y
```

### Clone Repository

```bash
git clone https://github.com/kavya0307/my-portfolio.git
```

### Build Image on EC2

```bash
sudo docker build -t portfolio-website .
```

### Run Container on EC2

```bash
sudo docker run -d -p 80:80 --name portfolio-container portfolio-website
```

## Learning Outcomes

* Static Website Hosting with AWS S3
* Content Delivery using CloudFront
* Version Control with Git & GitHub
* Docker Containerization
* Linux Server Management
* AWS EC2 Deployment
* Basic DevOps Workflow
* Cloud Application Deployment

## Author

Kavya
