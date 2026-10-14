# Ansible Practical: Install and Start Nginx

## Project Overview
This project demonstrates configuration management using Ansible on Ubuntu.

## Tools Used
- AWS EC2
- Ubuntu Linux
- Ansible
- YAML
- Nginx

## Tasks Performed
1. Installed Ansible on an Ubuntu EC2 instance.
2. Created an Ansible inventory file.
3. Tested connectivity using the Ansible ping module.
4. Created a playbook to update the APT cache.
5. Installed Nginx using the Ansible APT module.
6. Started and enabled the Nginx service.
7. Verified the service status.

## Commands Used
```bash
ansible --version
ansible all -i inventory.ini -m ping
ansible-playbook -i inventory.ini nginx.yml --syntax-check
ansible-playbook -i inventory.ini nginx.yml
sudo systemctl status nginx
```

## Learning Outcome
Learned Ansible inventory, playbooks, tasks, modules, YAML syntax, idempotency, and configuration management.
