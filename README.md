# DevOps Docker AWS Deployment

Deployed a public website on **AWS EC2 (Ubuntu)** and served it using **Docker + Nginx**.

## What I did
- Provisioned an AWS EC2 instance (Ubuntu)
- Configured Linux user access and basic server hardening
- Installed Docker and validated the runtime with `hello-world`
- Ran an Nginx container and exposed it on **port 80**
- Served a custom HTML page from inside the container

## Tech
AWS EC2 • Linux • Docker • Nginx • Git/GitHub

## Run locally
```bash
docker build -t nikunj-devops-site .
docker run -d -p 80:80 --name mywebsite nikunj-devops-site


Result:

Public URL (EC2 Public IP): http://18.130.225.224
