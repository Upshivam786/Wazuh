# 🛠️ Troubleshooting Wazuh

This page documents common issues I faced while working with Wazuh, and how I solved them.

---

## 1. Agent shows as *disconnected*
**Problem:** Agent added in the dashboard but status = disconnected.  
**Fix:**  
- Check agent service on the node:  
  ```bash
  sudo systemctl status wazuh-agent
If stopped, restart it:

sudo systemctl restart wazuh-agent


Ensure port 1514/UDP and 1515/TCP are open between manager and agent.

2. nano: command not found

Problem: Could not edit config files with nano.
Fix: Install nano or use vi:

sudo apt install nano -y

3. File changes not detected in dashboard

Problem: Created/deleted file but no alert visible.
Fix:

Ensure the directory is monitored in /var/ossec/etc/ossec.conf
Example:

<directories check_all="yes" report_changes="yes" realtime="yes">/home/ubuntu</directories>


Restart agent after editing config:

sudo systemctl restart wazuh-agent
