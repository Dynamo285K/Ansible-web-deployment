# Ansible Web Deployment 🚀

Automated provisioning and deployment of a static HTML website to an AWS EC2 instance using Ansible. 

## Features
* **System Prep (`base` role):** Updates packages and installs essential utilities (like Fail2ban).
* **Web Server (`nginx` role):** Installs and configures Nginx, managing the service state.
* **Deployment (`app` role):** Cleans the default web directory and automatically clones the latest website code from GitHub.

## Prerequisites
* Ansible installed on your local machine or Docker container.
* An active AWS EC2 instance (Ubuntu).
* A valid SSH private key (`.pem`) for server access.

## Usage

1. Create your inventory file based on the example:
   ```bash
   cp inventory.example.ini inventory.ini
