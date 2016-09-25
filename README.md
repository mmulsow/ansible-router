# ansible-router
Ansible playbook to configure Ubuntu 16.04 to work as a router for a small network.

Prereqs
-------
* A machine with two or more network connections, running Ubuntu 16.04.

Installation
------------
On your Ubuntu router run:
```bash
sudo apt -y install ansible
git clone https://github.com/mmulsow/ansible-router.git
cd ansible-router
vi playbook/group_vars/all.yml  # Configure as needed
ansible-playbook -i playbook/inventory -b -c local playbook/site.yml
reboot
```
