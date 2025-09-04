# 🛠️ Wazuh Installation Guide

This guide explains how to install **Wazuh Manager** and the **Wazuh Dashboard** on Ubuntu 22.04.

---

## 1. Update your system
```bash
sudo apt update && sudo apt upgrade -y


2. Download and run Wazuh installer
curl -sO https://packages.wazuh.com/4.12/wazuh-install.sh
sudo bash ./wazuh-install.sh -a



3. Access the Wazuh Dashboard

Open your browser and go to:

https://<your-manager-ip>


4. Verify installation

Check Wazuh services:

sudo systemctl status wazuh-manager
sudo systemctl status wazuh-dashboard


