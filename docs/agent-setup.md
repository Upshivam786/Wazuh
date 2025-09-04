# 🤝 Wazuh Agent Setup

This guide explains how to install and register a **Wazuh Agent** with your Wazuh Manager.

---

## 1. Install the Wazuh agent
On the endpoint (e.g., Ubuntu 22.04):
```bash
curl -sO https://packages.wazuh.com/4.12/wazuh-install.sh
sudo bash ./wazuh-install.sh -a


2. Register the agent

On the Wazuh Manager:

sudo /var/ossec/bin/manage_agents


Select option A to add a new agent.

Enter agent name, IP, and ID.

Copy the generated key.

On the Agent machine:

sudo /var/ossec/bin/manage_agents -i <your-agent-key>


Restart the agent:

sudo systemctl restart wazuh-agent

3. Verify connection

On the Manager:

sudo /var/ossec/bin/agent_control -ls


You should see the agent listed as active ✅


---

That way, your repo grows like a **practical handbook**.  
Later you can add:  
- `docs/file-monitoring.md` (test cases you did)  
- `docs/troubleshooting.md` (errors + fixes)  
