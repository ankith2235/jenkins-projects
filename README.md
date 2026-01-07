# Jenkins Projects – 2 Assignments

This repository contains Jenkins automation projects completed as part of my Cloud & DevOps training. These projects demonstrate experience with continuous integration (CI), branch-based deployment, and multi-node job execution.

---

## 🔹 Project 1: Git-Triggered Jenkins Pipeline

**Objective:**  
Automatically trigger a CI pipeline on code push without manual intervention.

**Tasks Performed:**
1. Installed and configured Jenkins on the master node
2. Configured a **Git Webhook** to trigger builds on a **develop** branch push
3. Created a Jenkins Pipeline job linked to a Git repository
4. Configured the pipeline to:
   - Clone source code to Jenkins workspace
   - Copy project files to a designated folder
5. Verified the build was automatically triggered on every commit to `develop`

**Outcome:**  
Successfully configured CI automation using Git hooks and Jenkins pipelines.

---

## 🔹 Project 2: Multi-Node Branch-Based Deployment

**Objective:**  
Deploy code to different servers depending on the branch pushed.

**Tasks Performed:**
1. Added **two Jenkins agent nodes** to the Jenkins master
   - One as a **Test node**
   - One as a **Prod node**
2. Created two Jenkins jobs:
   - **Push to Test**
   - **Push to Prod**
3. Configured job triggers:
   - Push to `test` branch → build job runs on **Test node**
   - Push to `master` branch → build job runs on **Prod node**
4. Configured each job to:
   - Pull the latest Git commit
   - Copy files to its respective server
5. Validated deployment by checking the file output on both servers

**Outcome:**  
Implemented branch-based CI/CD routing to target environments using Jenkins master-agent architecture.

---

## 🛠 Tools & Technologies Used
- Jenkins (Master + Agent nodes)
- Git & Git Webhooks
- Linux (Ubuntu)
- SCP / SSH for file copy
- GitHub / Bitbucket repository

---

## 🎯 Summary
These Jenkins projects demonstrate experience with:
- Git-triggered CI pipelines
- Master–agent node configuration
- Branch-based deployment rules
- Automated file delivery to test and production servers

