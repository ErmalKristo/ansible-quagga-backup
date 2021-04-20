# Backup Quagga Routing Suite configurations using Ansible and Git 

This is an Ansible configuration i use to backup Quagga Configurations and store it in Gitlab repository. We use this configuration in production so please feel free to use it.

The main files here are 
- ansible.cfg. We store some basic configurations here for Ansible like **host_key_checking=false** for disable ssh host check and **inventory=hosts** which tells Ansible where to find the inventory.
- group_vars/quagga.yaml where we specify the user/pass and the files to backup for the hosts in the group quagga.

├── ansible.cfg  
├── group_vars  
│   └── quagga.yaml  
├── hosts  
├── playbook.yaml  
└── vault  
    └── secrets.yaml  
