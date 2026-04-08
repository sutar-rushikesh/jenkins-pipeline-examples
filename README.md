
<h1 align="center">🚀 Jenkins Pipeline Examples</h1>

<p align="center">
Declarative Jenkins Pipelines | CI/CD Automation | DevOps Learning Repository
</p>

<p align="center">

<img src="https://img.shields.io/badge/Jenkins-Pipeline-red?style=for-the-badge&logo=jenkins"/>
<img src="https://img.shields.io/badge/DevOps-CI/CD-blue?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Linux-Automation-yellow?style=for-the-badge&logo=linux"/>
<img src="https://img.shields.io/badge/OpenSource-Learning-green?style=for-the-badge"/>

</p>

---

# 📌 Repository Overview

This repository contains **real Jenkins Declarative Pipeline examples** demonstrating common CI/CD automation patterns used by DevOps engineers.

The goal of this project is to help learners understand:

✔ Jenkins Pipeline syntax  
✔ CI/CD workflow automation  
✔ Parallel vs sequential pipeline execution  
✔ Job orchestration  
✔ Deployment automation

---

# 🧰 Tech Stack

| Tool | Purpose |
|-----|------|
| Jenkins | CI/CD Automation |
| Groovy | Pipeline scripting |
| Linux | Server environment |
| Nginx | Website hosting |

---

# 📂 Repository Structure

```
jenkins-pipeline-examples
│
├── parallel-pipeline
│   └── Jenkinsfile
│
├── parallel-sequential-pipeline
│   └── Jenkinsfile
│
├── job-trigger-pipeline
│   └── Jenkinsfile
│
├── workspace-pipeline
│   └── Jenkinsfile
│
├── website-deployment-pipeline
│   └── Jenkinsfile
│
└── README.md
```

---

# ⚙️ Jenkins Pipeline Examples

## 1️⃣ Parallel Pipeline

Runs multiple stages simultaneously to reduce pipeline runtime.

```groovy
stage('Parallel Execution') {
    parallel {
        stage('Build') {
            steps { echo "Building Application" }
        }
        stage('Test') {
            steps { echo "Running Tests" }
        }
    }
}
```

---

## 2️⃣ Job Trigger Pipeline

Triggers another Jenkins job from a pipeline.

```groovy
build 'child-job-name'
```

---

## 3️⃣ Custom Workspace Pipeline

Runs Jenkins pipeline inside a custom directory.

```groovy
agent {
    node {
        customWorkspace '/data/jenkins/workspace'
    }
}
```

---

# 🏗️ CI/CD Pipeline Architecture

![Pipeline Architecture](images/pipeline-architecture.png)

Pipeline Flow:

Developer → GitHub → Jenkins Trigger → Build & Test → Deploy → Live Website

---

# 🎬 DevOps CI/CD Animation

Example CI/CD workflow animation:

![CI/CD Pipeline](https://media.giphy.com/media/coxQHKASG60HrHtvkt/giphy.gif)

---

# 🚀 How to Run

Clone repository

```
git clone https://github.com/sutar-rushikesh/jenkins-pipeline-examples.git
```

Create a Jenkins Pipeline Job

1. Open Jenkins
2. Click **New Item**
3. Select **Pipeline**
4. Choose **Pipeline Script from SCM**
5. Add this repository URL
6. Run pipeline

---

# 📚 Learning Outcomes

✔ Jenkins Declarative Pipeline syntax  
✔ CI/CD pipeline automation  
✔ Pipeline parallel execution  
✔ Jenkins job orchestration  
✔ Basic deployment automation

---
# 📚 Jenkins Dashboard
<p align="center">
<img width="1920" height="1080" alt="Screenshot 2026-04-08 113544" src="https://github.com/user-attachments/assets/45654c36-6d5f-49f1-a6a2-3d21fba48fa9" />
</p>
sample-code-parallel
<p align="center">
<img width="1920" height="1080" alt="Screenshot 2026-04-08 113833" src="https://github.com/user-attachments/assets/3263797d-dcab-4c39-952f-b41b6d0a43e0" />
<img width="1920" height="1080" alt="Screenshot 2026-04-08 113845" src="https://github.com/user-attachments/assets/f8a68fe6-5bfe-4afa-8b21-1df22c14377c" />
</p>
sample-code-parallel+Sequential
<p align="center">
<img width="1920" height="1080" alt="Screenshot 2026-04-08 112852" src="https://github.com/user-attachments/assets/ea38ba61-173c-4208-81c6-d1b53b0136e2" />
<img width="1920" height="1080" alt="Screenshot 2026-04-08 112907" src="https://github.com/user-attachments/assets/7551b4d0-af04-41e5-b988-de6cc952af7e" />
</p>
Parallel + Sequential together
<p align="center">
<img width="1920" height="1080" alt="Screenshot 2026-04-08 112816" src="https://github.com/user-attachments/assets/89c31310-1c11-4245-b917-25746cf555a3" />
<img width="1920" height="1080" alt="Screenshot 2026-04-08 112722" src="https://github.com/user-attachments/assets/d5ad3e70-e0c1-4495-b3ab-51ec48d0b524" />
<img width="1920" height="1080" alt="Screenshot 2026-04-08 112831" src="https://github.com/user-attachments/assets/31d59df8-5464-48b9-ac19-1d6e96e3e156" />
</p>

simple-website-hosting-pipeline
<p align="center">
<img width="1920" height="1080" alt="Screenshot 2026-04-08 113605" src="https://github.com/user-attachments/assets/7ba7dfe8-df79-408c-9f90-3e7bcdd6d7c3" />
<img width="1920" height="1080" alt="Screenshot 2026-04-08 113619" src="https://github.com/user-attachments/assets/2be8635b-4057-40ed-a2ec-9ed894ebbf35" />
</p>


# 👨‍💻 Author

**Rushikesh Sutar**

DevOps Engineer | AWS | Kubernetes | Terraform | CI/CD

---

⭐ If this repository helped you, consider giving it a star!
