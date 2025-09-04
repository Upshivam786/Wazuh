# 🗂️ File Integrity Monitoring (FIM) with Wazuh

This guide shows how to test Wazuh’s file monitoring by creating, modifying, and deleting files.

---

## 1. Create a test file
On the monitored agent:
```bash
sudo tee /home/ubuntu/testfile.txt



2. Modify the file
sudo tee -a /home/ubuntu/testfile.txt

3. Delete the file
sudo rm /home/ubuntu/testfile.txt

4. Verify alerts in Wazuh Dashboard

Go to Wazuh Dashboard → Security Events and filter by:

syscheck.path

syscheck.event

rule.description

You should see events like:

added → file created

modified → file edited

deleted → file removed
