```{=html}
<!-- Animated Header -->
```
```{=html}
<h1 align="center">
```
🚀 Jenkins Pipeline Examples
```{=html}
</h1>
```
```{=html}
<p align="center">
```
Declarative Jenkins Pipelines \| CI/CD Automation \| DevOps Learning
Repository
```{=html}
</p>
```
```{=html}
<p align="center">
```
`<img src="https://img.shields.io/badge/Jenkins-Pipeline-red?style=for-the-badge&logo=jenkins"/>`{=html}
`<img src="https://img.shields.io/badge/DevOps-CI/CD-blue?style=for-the-badge"/>`{=html}
`<img src="https://img.shields.io/badge/Linux-Automation-yellow?style=for-the-badge&logo=linux"/>`{=html}
`<img src="https://img.shields.io/badge/OpenSource-Learning-green?style=for-the-badge"/>`{=html}
```{=html}
</p>
```

------------------------------------------------------------------------

# 📌 Repository Overview

This repository contains **practical Jenkins Declarative Pipeline
examples** demonstrating real-world CI/CD patterns used by DevOps
engineers.

It covers multiple pipeline strategies including:

✔ Parallel execution\
✔ Sequential stages\
✔ Job triggering\
✔ Custom workspace\
✔ Website deployment automation

------------------------------------------------------------------------

# 🧰 Tech Stack

  Tool      Purpose
  --------- --------------------
  Jenkins   CI/CD Automation
  Groovy    Pipeline scripting
  Linux     Server environment
  Nginx     Website hosting

------------------------------------------------------------------------

# 📂 Repository Structure

    jenkins-pipeline-examples
    │
    ├── parallel-pipeline
    │   └── Jenkinsfile
    ├── parallel-sequential-pipeline
    │   └── Jenkinsfile
    ├── job-trigger-pipeline
    │   └── Jenkinsfile
    ├── workspace-pipeline
    │   └── Jenkinsfile
    ├── simple-website-deployment
    │   └── Jenkinsfile
    └── README.md

------------------------------------------------------------------------

# ⚙️ Jenkins Pipeline Examples

## 1️⃣ Custom Workspace Pipeline

Runs the Jenkins pipeline inside a **custom directory**.

    agent {
        node {
            customWorkspace '/data/jenkins/workspace'
        }
    }

------------------------------------------------------------------------

## 2️⃣ Job Trigger Pipeline

One Jenkins pipeline **triggers another job**.

    build 'child-job-name'

------------------------------------------------------------------------

## 3️⃣ Parallel Pipeline

Runs multiple stages simultaneously.

    parallel {
        stage('Build') { steps { echo "Building" } }
        stage('Test') { steps { echo "Testing" } }
    }

------------------------------------------------------------------------

## 4️⃣ Parallel + Sequential Pipeline

Combination of **parallel execution followed by sequential stages**.

Example workflow:

    Build + Test (Parallel)
            ↓
    Security Scan
            ↓
    Deploy

------------------------------------------------------------------------

## 5️⃣ Simple Website Deployment Pipeline

Automates deployment of a **static website using Nginx**.

Pipeline tasks:

✔ Install Nginx\
✔ Deploy website files\
✔ Restart Nginx service

------------------------------------------------------------------------

# 🏗️ CI/CD Pipeline Architecture

``` mermaid
flowchart TD

A[Developer Push Code] --> B[Git Repository]
B --> C[Jenkins Pipeline Trigger]
C --> D{Pipeline Execution}

D --> E[Build Stage]
D --> F[Test Stage]

E --> G[Security Scan]
F --> G

G --> H[Deploy Application]

H --> I[Nginx Web Server]

I --> J[Website Live]
```

------------------------------------------------------------------------

# 🚀 Pipeline Workflow

    Code Commit
         ↓
    Jenkins Trigger
         ↓
    Parallel Build & Test
         ↓
    Security Scan
         ↓
    Deploy Application
         ↓
    Restart Nginx
         ↓
    Website Live

------------------------------------------------------------------------

# 🔧 Prerequisites

Before running pipelines ensure:

-   Jenkins Installed
-   Linux based Jenkins Agent
-   Required permissions configured

For deployment pipelines:

    sudo visudo

Add:

    jenkins ALL=(ALL) NOPASSWD: ALL

------------------------------------------------------------------------

# 📚 Learning Outcomes

✔ Jenkins Declarative Pipelines\
✔ Parallel vs Sequential execution\
✔ Job orchestration in Jenkins\
✔ Workspace customization\
✔ CI/CD deployment automation

------------------------------------------------------------------------

# 👨‍💻 Author

**Rushikesh Sutar**

DevOps Engineer\
AWS \| Kubernetes \| Terraform \| CI/CD \| Linux

------------------------------------------------------------------------

# ⭐ Support

If this repository helped you:

⭐ Star the repository\
🍴 Fork it\
📢 Share with DevOps learners
