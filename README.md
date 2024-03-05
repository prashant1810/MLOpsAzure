# MLOpsAzure

1. Setup GitHub Repository
   - new environment
   - setup.py
   - requirements.txt

2. Src folder and build the package

- conda create -p venv python==3.8 -y
- conda activate venv/
- pip install -r requirements.txt
- git add .
- git status
- git commit -m "Setup.py and requirements.txt"
- git push -u origin main

- Added elastic beans file in .ebextensions folder

Docker Commands
- docker build -t studentperformance
- docker images
- docker run -p 5000:5000 studentperformance
- docker ps
- docker stop
- docker login
- docker image rm -f studentperformance
- docker build -t prash/studentperformance
- docker tag studentperformance prash/studentperformance
- docker push prash/studentperformance:latest
- docker compose up

Steps:
1. Docker Build
2. Github Workflow
3. IAM User AWS (prash1)
4. Ec2 instance creation
 - Create specific user EC2fullaccess, ContainerFullAccess
 - Add security inbounds for Custom TCP and port 8080

211125634833.dkr.ecr.us-east-1.amazonaws.com/studentperformace

Docker setup in ec2
- sudo apt-get update -y
- sudo apt-get upgrade
- curl -fsSL https://get.docker.com -o get-docker.sh
- sudo sh get-docker.sh
- sudo usermod -aG docker ubuntu
- newgrp docker

Go to GitHub Settings/Actions/Runner 
- create for EC2 for runner for linux

Goto Secrets/Actions
