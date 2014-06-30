development.environments
========================

My development environments

#Getting Started

###Requirements

[Ansible](http://www.ansible.com/)

Install ansible:

```
sudo apt-get install apt-add-repository
sudo apt-add-repository ppa:rquillo/ansible
sudo apt-get update
sudo apt-get install ansible
```

#Run

Change user in provisioning/playbook.yml and execute:

```
ansible-playbook provisioning/playbook.yml -i production_hosts -K 
```
