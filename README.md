#  🚀 SharePoint Video Downloader

## Overview
This is a self-hosted SharePoint video downloader that allows users to download SharePoint-hosted videos, even when they have view-only permissions. The project leverages Flask, Docker, and Nginx reverse proxy to provide a secure and efficient solution.

## 🔧 Features
- 📥 Download view-only SharePoint videos
- 🔀 Reverse Proxy (Nginx) for secure access
- 🚀 Dockerized deployment with Docker Compose
- 🔄 CI/CD integration using GitHub Actions
- 🔒 SSL encryption support for secure connections
- 📂 File browser UI for managing downloaded files

## 🏗 Tech Stack
- 🐍 Flask (API Backend)
- 🔥 SocketIO (Real-time updates)
- 🐳 Docker & Docker Compose (Containerization)
- 🌐 Nginx Reverse Proxy (Secure access)
- 🚀 GitHub Actions (CI/CD automation)
- 🖥 Ubuntu VPS (Hosting environment)

## 📜 Prerequisites
1. Ubuntu VPS with:
   - Docker
   - Docker Compose
   - Git
2. Domain name pointing to your VPS IP
3. SSL certificates (from Cloudflare or similar)
4. GitHub account for deployment

## 🚀 Deployment Guide

### 1️⃣ Domain Configuration
1. Point your domain to your VPS IP address
2. Set up Cloudflare or other SSL provider
3. Obtain SSL certificate and private key

### 2️⃣ GitHub Repository Setup
1. Fork or clone this repository
2. Configure GitHub Secrets:
   - `INSTANCE_IP`: Your VPS IP
   - `INSTANCE_USERNAME`: VPS SSH username
   - `SSH_PRIVATE_KEY`: SSH private key for deployment
   - `GHUB_USERNAME`: Your GitHub username
   - `TOKEN`: GitHub personal access token
   - `SSL_CERT`: SSL certificate content
   - `SSL_KEY`: SSL private key content

### 3️⃣ Nginx Configuration
Edit the domain names in:
- `nginx/reverse-proxy/app.conf`: Change `app.techdevops.live` to your app domain
- `nginx/reverse-proxy/file.conf`: Change `files.techdevops.live` to your file browser domain

### 4️⃣ Deployment
The application will automatically deploy when you push to the main branch.

To verify deployment:
1. Check GitHub Actions tab for deployment status
2. Verify containers are running on your VPS:
```bash
docker ps
```

### 5️⃣ Access
- Web Interface: `https://your-app-domain`
- File Browser: `https://your-file-domain`

## 🔒 Security Notes
- All traffic is encrypted using SSL/TLS
- Nginx reverse proxy provides additional security
- Containers run in isolated network
- Regular updates via automated deployment

## 📞 Support
Create an issue on GitHub for:
- Deployment questions
- Configuration help
- Bug reports


## 📜 License

This project is licensed under the [MIT License](LICENSE).

<br><br>

# 💰 You can help me by Donating
<img align="center" alt="Coding" width="400" src="https://github.com/pasinduljay/pasinduljay/blob/main/Resources/user2.gif">

<a href="https://buymeacoffee.com/pasinduljay" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" height="50px" ></a>
<a href="https://paypal.me/980822" target="_blank"><img src="https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white" alt="Buy Me A Coffee" height="50px" >
<br><br>