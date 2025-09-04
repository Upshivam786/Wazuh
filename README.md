# Wazuh
# 🚀 Wazuh Setup & Hands-on Lab

This repository documents my step-by-step work with **Wazuh**, including installation, agent setup, file integrity monitoring, and test cases.  
It is meant as a practical guide for anyone who wants to quickly set up and experiment with Wazuh.

---

## 📌 Contents
- [Installation Guide](01-installation.md) – How to install Wazuh manager and dashboard  
- [Agent Setup](02-agent-setup.md) – Registering agents and verifying connection  
- [File Monitoring Test](03-file-monitoring.md) – Creating/deleting files and checking alerts  
- [Troubleshooting](04-troubleshooting.md) – Fixes for common issues  

---

## ⚡ Quick Start (Ubuntu 22.04)

Install Wazuh manager + dashboard in one command:

```bash
curl -sO https://packages.wazuh.com/4.12/wazuh-install.sh
sudo bash ./wazuh-install.sh -a
