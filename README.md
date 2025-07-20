# Ansible


This will be my awesome Ansible repository!
Update in 2025

## 🧪 To Bootstrap a Machine

Use this playbook to prepare a new node for Homelab inclusion:

```bash
ansible-playbook playbooks/bootstrap.yml --ask-become-pass --tags bootstrap -l <host>

ansible-playbook playbooks/bootstrap.yml --ask-become-pass --tags bootstrap -l k3s-ashborn.domain.io

This will:

Create the user ashborn
Install your SSH key
Set timezone, hostname, base packages
Configure SSH security
Optionally upgrade all packages (based on unattended_upgrades)
