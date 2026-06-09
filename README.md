# ☁️ AWS Cloud Resume Portal with CI/CD Pipeline

A fully automated cloud-hosted resume website built using AWS and GitHub. This project demonstrates modern DevOps practices by implementing a Continuous Integration and Continuous Deployment (CI/CD) pipeline that automatically deploys website updates from GitHub to Amazon S3.

---

## 🚀 Project Overview

This project hosts a personal portfolio website on Amazon S3 and automates deployments using AWS CodePipeline and AWS CodeBuild.

Whenever changes are pushed to the GitHub repository, the pipeline automatically:

1. Detects code changes
2. Pulls the latest source code
3. Builds the project
4. Deploys updated files to Amazon S3
5. Updates the live website

This eliminates manual deployments and follows real-world cloud engineering and DevOps workflows.

---

## 🏗️ Architecture Diagram

![Architecture](screenshots/01-project-architecture-diagram.png)

---

## ☁️ AWS Services Used

| Service | Purpose |
|----------|----------|
| Amazon S3 | Static website hosting |
| AWS CodePipeline | CI/CD orchestration |
| AWS CodeBuild | Build automation |
| IAM | Access management |
| GitHub | Source code repository |
| GitHub App Connection | Source integration with AWS |

---

## 📁 Project Structure

```text
aws-cloud-resume-portal/
│
├── index.html
├── styles.css
├── script.js
├── buildspec.yml
├── README.md
│
└── screenshots/
```

---

## ✨ Features

- Static website hosted on Amazon S3
- Version-controlled using GitHub
- Automated deployment pipeline
- Build automation using CodeBuild
- GitHub integration via GitHub App
- Zero-downtime deployments
- Beginner-friendly DevOps workflow
- AWS Free Tier compatible

---

# 📸 Implementation Screenshots

---

## GitHub Repository

### Repository Created

![GitHub Repository](screenshots/02-github-repository-created.png)

### Project Files

![GitHub Files](screenshots/03-github-project-files.png)

---

## Amazon S3 Setup

### S3 Bucket Created

![S3 Bucket](screenshots/04-s3-bucket-created.png)

### Static Website Hosting Enabled

![Static Hosting](screenshots/05-s3-static-hosting-enabled.png)

### Bucket Policy Configuration

![Bucket Policy](screenshots/06-s3-bucket-policy.png)

### Live Website

![Live Website](screenshots/07-s3-live-website.png)

---

## AWS CI/CD Configuration

### CodeBuild Project

![CodeBuild](screenshots/08-codebuild-project-created.png)

### Source Stage Configuration

![Source Stage](screenshots/09-source-stage-config.png)

### CodePipeline Configuration

![Pipeline](screenshots/10-codepipeline-created.png)

---

## Successful CI/CD Deployment

### Pipeline Success

![Pipeline Success](screenshots/11-codepipeline-success.png)

### Automatic Website Update

![Auto Deployment](screenshots/12-website-auto-updated.png)

---

# 🔄 CI/CD Workflow

```text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
AWS CodePipeline
    │
    ▼
AWS CodeBuild
    │
    ▼
Amazon S3 Website
    │
    ▼
End Users
```

---

## 🛠️ Deployment Process

### Step 1

Developer pushes code changes:

```bash
git add .
git commit -m "Website update"
git push origin main
```

### Step 2

GitHub notifies AWS CodePipeline.

### Step 3

CodePipeline retrieves the latest source code.

### Step 4

CodeBuild processes the build instructions from:

```text
buildspec.yml
```

### Step 5

Updated website files are deployed to Amazon S3.

### Step 6

The live website reflects the new changes automatically.

---

## 🎯 Skills Demonstrated

### AWS

- Amazon S3
- AWS CodePipeline
- AWS CodeBuild
- IAM
- GitHub Integration

### DevOps

- CI/CD Pipelines
- Automated Deployments
- Source Control
- Build Automation
- Deployment Automation

### Cloud Engineering

- Static Website Hosting
- Cloud Architecture Design
- AWS Resource Management
- Infrastructure Troubleshooting

---

## 💰 Cost Optimization

This project was designed using AWS Free Tier eligible services.

Resources used:

- Amazon S3
- CodePipeline
- CodeBuild
- IAM

Always monitor AWS billing and remove unused resources after testing.

---

## 🧹 Cleanup

To avoid charges:

1. Delete CodePipeline
2. Delete CodeBuild Project
3. Delete S3 Bucket
4. Remove GitHub Connection
5. Verify no resources remain active

---

## 📚 Key Learnings

- Building cloud-hosted web applications
- Implementing CI/CD pipelines
- Integrating GitHub with AWS
- Automating deployments
- Managing AWS permissions and roles
- Troubleshooting deployment failures

---

## 👨‍💻 Author

**Jeet Zala**

Aspiring Cloud Engineer focused on AWS, DevOps, Infrastructure Automation, and Cloud Operations.

---

⭐ If you found this project helpful, feel free to fork the repository and give it a star.
