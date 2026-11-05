# Laboratory Activity 08: The Cloud Security Engineer

## Mission Overview
This laboratory covers host-based cloud security using the Uncomplicated Firewall (UFW) in an Ubuntu environment. The objective is to secure an exposed public container instance by establishing a strict Default Deny baseline and selectively permitting legitimate SSH and web traffic.

## Objectives
- Implement the Principle of Least Privilege (PoLP) and reduce host attack surfaces.
- Audit active service ports on an Ubuntu host.
- Configure UFW with a Default Deny inbound policy.
- Configure granular firewall rules for TCP ports 22 (SSH) and 8080 (Web App).
- Document configuration commands and security baselines in Markdown.

## Commands Executed
| Purpose | Command |
| :--- | :--- |
| Deploy Container | `docker run -d -p 8080:80 --name secure-web-app nginx` |
| Test Connectivity | `curl -I http://localhost:8080` |
| Permit SSH | `sudo ufw allow ssh` |
| Set Default Incoming | `sudo ufw default deny incoming` |
| Set Default Outgoing | `sudo ufw default allow outgoing` |
| Enable Firewall | `sudo ufw enable` |
| Open Port 8080 | `sudo ufw allow 8080/tcp` |
| Audit Rules | `sudo ufw status verbose` / `sudo ufw status numbered` |

## Skills Learned
- Linux host-level packet filtering with `ufw`.
- Preventing administrative lockouts during firewall initialization.
- Applying least-privilege network policies to microservices.
- Systematic verification of port accessibility using CLI tools.
