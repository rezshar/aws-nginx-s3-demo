# AWS Demo Project: Nginx + S3 Website

This is my **simple AWS project** as part of my DevOps/SRE learning journey.  
The goal was to build a simple **web application** hosted on **EC2 (Nginx)** and serving static files from **S3**.

---

**Flow:**
1. User requests website → EC2 Public IP
2. Nginx serves files from local directory
3. Files are synced from **S3 bucket** → EC2

---

## 🚀 Steps to Reproduce

### 1️⃣ Create IAM User
- Permissions: `AmazonS3FullAccess`, `AmazonEC2FullAccess`

### 2️⃣ Create S3 Bucket
```bash
aws s3 mb s3://devops-reza-demo
