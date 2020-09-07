Ansible playbook: Post Ubuntu workstation installation 
=========
[![Build Status](https://travis-ci.com/gmarokov/ansible-playbook-postinstall-ubuntu.svg?branch=master)](https://travis-ci.com/gmarokov/ansible-playbook-postinstall-ubuntu)

Post Ubuntu installation Ansible script for provisioning dev machine.

## Installation
1. Install Ansible 
`sudo dnf install ansible`
2. Add entry to your hosts in `/etc/ansible/hosts`:
```
cat <<EOT >> /etc/ansible/hosts
[localhost] 
127.0.0.1
EOT
```
3. Become root:
`sudo -i`

## Usage
1. Run the following command to pull and run the playbook: `ansible-pull -U https://github.com/gmarokov/ansible-playbook-postinstall-ubuntu.git`

## Script details 

### Pre tasks
- Update system

### Tasks

#### Install apt packages
- Git
- CopyQ
- Gnome Tweaks

#### Install Snap packages
- Visual Studio Code
- Postman
- Dotnet SDK 2.1
- Node.js 12
- Docker
- Firefox
- Spotify
