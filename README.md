# ansible-router
Ansible playbook to configure Ubuntu 16.04 to work as a router for a small network.

Prereqs
-------
* A machine with two or more network connections, running Ubuntu 16.04.

Installation
------------
On your Ubuntu router run:
```bash
sudo apt-get -y install git python-virtualenv
virtualenv router-env
. router-env/bin/activate
git clone https://github.com/mmulsow/ansible-router.git
cd ansible-router
pip install -r requirements.txt
vi playbook/group_vars/all.yml  # Configure as needed
ansible-playbook -i playbook/inventory -b -c local playbook/site.yml
```
