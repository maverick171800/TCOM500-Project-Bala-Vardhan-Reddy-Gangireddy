Project Objective:

Create and implement a central control node-based  Ansible-based automation system to configure and manage several Linux hosts.  

This comprises:

Automated SSH key management
Baseline hardening (firewall, NTP, logging, users, and packages)  
Patching and updating the operating system

Design Overview:

Ansible host (Ubuntu or AWS EC2) is the control node.
Three or more Linux servers (AWS or Raspberry Pi) are managed nodes.
Inventory: either dynamic (AWS) or static (Pi)

Roles:

  Manage authorized keys using SSH keys.
  Users, firewall, NTP, and packages are the baseline.
  Patching: reboots and OS updates

Requirements:

Ansible 2.10+
Python 3.x
SSH key-based node communication
Git installed for version management
AWS EC2 or local virtual machines for testing

Next Steps

1. Configure the infrastructure (hosts + control node)  
2. Establish Ansible roles and inventories  
3. Create playbooks (keys.yml, update.yml, and site.yml).  
4. Test, Document, and push updates  

