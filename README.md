# Flask CI/CD with Jenkins and Codeberg

# Project Overview
A simple Flask app deployed via Jenkins triggered by Codeberg webhooks.

# Technologies Used
- Python Flask
- Jenkins
- GitHub Actions
- Codeberg

# Setup Instructions

# 1. Jenkins Setup
- Installed on Ubuntu using apt
- Configured to pull Codeberg repo on push

#  2. Webhook
- Codeberg webhook points to: `http://<IP>:8080/github-webhook/`

# 3. CI/CD Workflow
- Triggered on push
- Jenkins:
  - Clones repo
  - Installs dependencies
  - Restarts app

# Notes
- App runs on port 5000
- You can Dockerize it optionally
