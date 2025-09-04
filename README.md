# 🚀 Wazuh Setup & Hands-on Lab

This repository documents my step-by-step work with **Wazuh**, including installation, agent setup, file integrity monitoring, and troubleshooting.  
It serves as a **hands-on lab guide** for anyone who wants to quickly set up and experiment with Wazuh.

---

## 📂 Documentation

- [🛠️ Installation Guide](docs/installation.md)  
  Install Wazuh Manager and Dashboard on Ubuntu 22.04.

- [🤝 Agent Setup](docs/agent-setup.md)  
  Register agents and verify their connection.

- [📂 File Monitoring](docs/file-monitoring.md)  
  Configure Wazuh to detect file creation, modification, and deletion.

- [🚑 Troubleshooting](docs/troubleshooting.md)  
  Fixes for common issues.

---

## ⚡ Quick Start (Ubuntu 22.04)

Install Wazuh manager + dashboard in one command:

```bash
curl -sO https://packages.wazuh.com/4.12/wazuh-install.sh
sudo bash ./wazuh-install.sh -a
