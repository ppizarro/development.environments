#My development environments

###Requirements

1. [Ansible](http://www.ansible.com/)
1. [VirtualBox](http://www.virtualbox.org/)
1. [Vagrant](http://www.vagrantup.com/)

###Getting Started

1. Clone the project

```
$ git clone https://github.com/ppizarro/development.environments.git
$ cd development.environments
```

1. Install ansible:

```
sudo apt-get install apt-add-repository
sudo apt-add-repository ppa:rquillo/ansible
sudo apt-get update
sudo apt-get install ansible
```

###Provisioning

Change user in provisioning/playbook.yml and execute:

```
ansible-playbook provisioning/playbook.yml -i provisioning/production_hosts -K 
```

