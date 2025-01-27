# Windows RDP GitHub Actions

This repository provides a GitHub Actions workflow that sets up a Windows Remote Desktop (RDP) connection using Ngrok.

## 🚀 Setup Instructions

1. Fork this repository
2. Go to your fork's Settings > Secrets and Variables > Actions
3. Add a new repository secret:
   - Name: `NGROK_AUTH_TOKEN`
   - Value: Your Ngrok authtoken (get it from https://dashboard.ngrok.com/auth)

## 📋 Usage

1. Go to the Actions tab in your forked repository
2. Select the "Windows RDP" workflow
3. Click "Run workflow"
4. Wait for the workflow to start and show the RDP connection details
5. Use any RDP client (like Windows Remote Desktop) to connect using the provided details:
   - Host: (Provided by workflow)
   - Username: rdpuser
   - Password: P@ssw0rd!123

## ⚠️ Important Notes

- The RDP session will remain active for 6 hours (GitHub Actions limit)
- Do not share your RDP credentials with others
- The connection is tunneled through Ngrok for security
- Your Ngrok authtoken should be kept secret

## 🔒 Security

- A new user account is created for each session
- The RDP connection is tunneled through Ngrok's secure servers
- Credentials are randomly generated for each session
- The workflow uses Windows Server 2019 as the base image

## ⚡ Features

- Windows Server 2019
- 2-core CPU
- 7 GB RAM
- 14 GB SSD space
- Full administrator access
- Ngrok tunneling for secure access

## 📝 License

This project is for educational purposes only. Do not use for any commercial or unauthorized purposes.
