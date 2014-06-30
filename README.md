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

###Roles

 1. Common
  * Update apt
  * Install language-pack-en, gcc, g++ and make

 1. Git
  * Install git
  * Set git user.name
  * Set git user.email
  * Set git push.default
  
 1. vim
  * Install vim and exuberant-ctags
  * Install my.vim

 1. nodejs
  * Add the node.js PPA
  * Install node.js and npm
  * Install Mocha node.js package globally
  * Install Jasmine node.js package globally
  * Install Grunt node.js package globally

 1. front-end
  * Install Bower node.js package globally
  * Install Karma node.js package globally
  * Install Yeoman node.js package globally
  * Install Angular.js generator

