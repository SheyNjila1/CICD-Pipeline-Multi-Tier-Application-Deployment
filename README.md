# CICD-Pipeline-Multi-Tier-Application-Deployment
In this project, I will use the CI/CD Pipeline for A Multi-Tier Application Deployment using Jenkins. In this project, I will integrate Maven, SonarQube, Nexus, Docker , Ansible, Kubernetes, Prometheus, Grafana, and SNS for Jira integration.  

# Step by step implementation of Jenkins Pipeline Project
## 1. Create a GitHub Repository Jenkins-CI/CD-Pipeline-Project and push the code in this branch(main) to your remote repository (your newly created repository).

Go to GitHub (github.com)
Login to your GitHub Account
Create a Repository called "Jenkins-CICD-Project"
Clone the Repository in the "Repository" directory/folder in your local
Download the code in in this repository "Main branch":
## 2. Install Docker, Jenkins, Java, git, and AWS cli in Ubuntu
```
# Install and configure Docker:
sudo apt update -y 
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker.service
sudo systemctl status docker.service

# Install java 11
sudo apt update -y
sudo apt install openjdk-11-jdk -y

# Install and configure Jenkins: --->How to Install Jenkins on Ubuntu 20.04 | Linuxize
wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt update -y
sudo apt install jenkins -y
sudo systemctl start jenkins
sudo usermod -aG docker jenkins
sudo systemctl restart docker.service
sudo echo "jenkins ALL=(ALL) NOPASSWD:ALL" | sudo tee /etc/sudoers.d/jenkins   # Also CHeck-->https://gist.github.com/desferreira/2dced846c6e6e9cbf67f79227d613e7c
sudo su - jenkins 

# Setup Jenkins to start at boot
sudo apt install git -y
sudo apt install python -y
sudo apt install python-pip -y
pip3 install ansible -y

# Install awscli---->https://docs.aws.amazon.com/cli/v1/userguide/install-linux.html 
sudo apt install wget -y
sudo apt update -y
sudo apt install unzip 
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install

```

## 3. SonarQube


## 4. Nexus

## 5. EC2 (Dev, Stage, Prod)


## 6. Prometheus

## 7. Grafana


## 8. Slack

## 9. Configure Prometheus

## 10. Configure Grafana

## 11. Configure The "Node Exporter" on the "Jenkins-Maven-Ansible", "Nexus" and "SonarQube" instances


## 12. Update the Prometheus config file and include all the IP

## 13. 

