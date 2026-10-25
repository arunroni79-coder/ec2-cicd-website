# ec2-cicd-website
Automated website deployment using github actions and aws ec2
# Automated Website Deployment on AWS EC2 Using GitHub Actions

## 📌 Project Overview
This project demonstrates an automated website deployment pipeline using AWS EC2, Apache HTTP Server, and GitHub Actions. Whenever changes are pushed to the `main` branch, GitHub Actions automatically transfers the updated website files to the EC2 instance and deploys them.

## 🛠️ Technologies Used
- **AWS EC2** – Hosts the website on a cloud server.
- **Apache HTTP Server** – Serves the website to users.
- **Git & GitHub** – Manages source code and version control.
- **GitHub Actions** – Automates the CI/CD workflow.
- **SSH** – Provides secure remote access for deployment.
- **Linux** – Supports server configuration and management.
- **GitHub Secrets** – Stores deployment credentials securely.

## ⚙️ How It Works
1. Create and configure an AWS EC2 instance.
2. Install and configure Apache HTTP Server.
3. Upload the website's `index.html` file to GitHub.
4. Configure GitHub Actions to connect to EC2 using SSH.
5. Store the required host, username, and private key in GitHub Secrets.
6. Push changes to the `main` branch.
7. GitHub Actions automatically deploys the updated website to Apache.

## 🚀 Key Features
- Automated deployment on every qualifying push to `main`.
- Cloud-based website hosting using AWS EC2.
- Continuous Integration and Continuous Deployment (CI/CD).
- Secure credential management using GitHub Secrets.
- Reduced manual effort in updating website files.

## 📂 Repository Structure
```text
ec2-cicd-website/
├── .github/
│   └── workflows/
│       └── deploy.yml
├── index.html
├── .gitignore
└── README.md
```

## 🔒 Security Notes
- Store private SSH keys in GitHub Secrets, not in the repository.
- Use `.gitignore` to help prevent private-key files from being committed.
- Restrict SSH access to trusted IP addresses or use AWS Systems Manager Session Manager where appropriate.
- Keep AWS credentials and other sensitive information out of source code.

## 🎯 Learning Outcomes
- Learned to launch and configure an AWS EC2 instance.
- Practiced Linux server administration and Apache configuration.
- Implemented an automated CI/CD pipeline using GitHub Actions.
- Used SSH and GitHub Secrets for deployment authentication.
- Understood how code changes can be automatically deployed to a cloud-hosted website.

## 👨‍💻 Author
Created as a hands-on cloud computing and DevOps project to practice AWS infrastructure, Linux, web hosting, and CI/CD automation.

