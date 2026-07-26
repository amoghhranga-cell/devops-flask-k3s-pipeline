# 🚀 End-to-End DevOps CI/CD Pipeline using AWS, Terraform, Docker, K3s & GitHub Actions

## Project Overview

This project demonstrates a complete end-to-end DevOps CI/CD pipeline for deploying a Python Flask application on AWS.

The infrastructure is provisioned using Terraform, the application is containerized with Docker, deployed to a K3s Kubernetes cluster running on an AWS EC2 instance, and automated using GitHub Actions. AWS CloudWatch is used to monitor the infrastructure.

---

## Tech Stack

- AWS EC2
- Terraform
- Docker
- K3s Kubernetes
- GitHub Actions
- Python Flask
- AWS CloudWatch
- Git
- Linux (Ubuntu)


---

## Project Structure

```text
devops-flask-k3s-pipeline/
│
├── app/
│   ├── app.py
│   ├── Dockerfile
│   ├── deployment.yaml
│   ├── service.yaml
│   └── requirements.txt
│
├── terraform/
│   └── main.tf
│
└── .github/
    └── workflows/
        └── deploy.yml
```

---

## Features

- Infrastructure provisioning using Terraform
- Dockerized Python Flask application
- Kubernetes deployment using K3s
- Automated CI/CD pipeline with GitHub Actions
- Docker image build and push
- Automated deployment to AWS EC2
- Infrastructure monitoring with AWS CloudWatch

---

## CI/CD Workflow

1. Developer pushes code to GitHub.
2. GitHub Actions automatically triggers the workflow.
3. Docker builds the Flask application image.
4. The Docker image is pushed to Docker Hub.
5. GitHub Actions connects to the AWS EC2 instance using SSH.
6. The latest image is deployed to the K3s Kubernetes cluster.
7. Kubernetes updates the running application.
8. AWS CloudWatch monitors the EC2 instance and application metrics.

---

## Monitoring

AWS CloudWatch is used to monitor the health and performance of the EC2 instance.

The dashboard includes the following metrics:

- CPU Utilization
- Network In
- Network Out
- Status Check Failed

These metrics help monitor resource utilization, network traffic, and instance health.


## Learning Outcomes

Through this project, I gained hands-on experience with:

- Infrastructure as Code (Terraform)
- Docker containerization
- Kubernetes deployment using K3s
- CI/CD pipeline automation with GitHub Actions
- AWS EC2 deployment
- CloudWatch monitoring and dashboards
- Linux server administration
- Git and GitHub workflows


---

## Author

Amogh H R

- GitHub: https://github.com/amoghhranga-cell

If you found this project helpful or have any suggestions, feel free to connect or open an issue.
