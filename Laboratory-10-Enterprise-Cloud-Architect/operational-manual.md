# CloudNova Enterprise Architecture - Operational Manual

## 1. System Overview
This repository contains the Infrastructure as Code (IaC) deployment for CloudNova's enterprise application stack, featuring a containerized two-tier deployment (WordPress Application + MariaDB), localized firewall isolation, and automated daily backup routines.

## 2. Network & Port Allocation
* **Host Port 22/tcp:** Secure Shell (SSH) access
* **Host Port 8080/tcp:** External HTTP entry point mapped to the Web Application
* **Internal Docker Network (`enterprise_backend_net`):** MariaDB listens on `database:3306` inside the private bridge; external access is blocked.

## 3. Provisioning & Deployment
1. Clone the repository and navigate to the directory:
   ```bash
   cd Laboratory-10-Enterprise-Cloud-Architect
