# ansible
All things ansible

# Install ansible
sudo apt install ansible

# Usage
Install ansible, then

## With ansible-pull

  ansible-pull -U <your:token>@github.com/scraptop/ansible.git 

or point to a local directory:

  ansible-pull -U ~/workspace/ansible-soup

## With ansible-push

  ansible-playbook tmux.yml -vvv -K

Where -K means prompt for sudo password

# Usage without git

Requires to specify localhost in header of playbooks, in inventory or on cmdline

  ansible-playbook playbook.yml 

Example header:

  - hosts: 127.0.0.1 
  connection: local
