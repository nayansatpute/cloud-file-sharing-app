# ☁️ Cloud File Sharing App using AWS

A serverless cloud file sharing web app built with AWS Lambda, Amazon S3, and Netlify.

## 🔗 Live Demo
👉 [Click here to open the app](https://ornate-tiramisu-39a73b.netlify.app)

## 🛠️ Tech Stack
- **Frontend:** HTML, CSS, JavaScript (hosted on Netlify)
- **Compute:** AWS Lambda (Python) — generates pre-signed URLs
- **Storage:** Amazon S3 — stores uploaded files
- **Security:** AWS IAM roles, CORS policies, pre-signed URLs

## ⚙️ How It Works
1. User selects a file → frontend calls Lambda
2. Lambda generates a temporary pre-signed S3 URL
3. Browser uploads file **directly to S3** (no server middleman)
4. Same flow in reverse for downloads

## 🏗️ Architecture
Browser → Lambda (get pre-signed URL) → S3 (direct upload/download)

## ✨ Features
- Upload any file to AWS S3
- Download files from AWS S3
- Serverless — no backend server needed
- Secure time-limited pre-signed URLs
