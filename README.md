# 🚀 Hybrid Docker Compose Deployment with Ansible

This project demonstrates how to use **Ansible** to deploy a `docker-compose` service to both a **on-premises** and a **cloud Linux server**, with automated container shutdown to optimize costs.

---

## 🧰 What This Shows

✅ Ansible-based deployment of Docker + Compose  
✅ Automated service provisioning on both cloud and on-prem  
✅ Role-based and inventory-driven architecture  
✅ Scheduled container shutdown using `cron`  
✅ Infrastructure as Code (IaC) using modern DevOps practices

---

## 🌐 Supported Environments

- RHEL/CentOS 8/9 (or compatible)
- Cloud servers (e.g., AWS, Azure, GCP)
- On-prem VMs or bare metal

---

## 🏗️ Project Structure

```bash
deploy/
├── inventory.ini          # Define on-prem and cloud groups
├── deploy_service.yml     # Main playbook to deploy container
├── group_vars/all.yml     # Global variables (e.g., app_dir)
└── roles/
    └── service/
        ├── tasks/main.yml        # Ansible automation logic
        └── files/docker-compose.yml # Sample app to deploy

