Ansible playbook: Post Ubuntu workstation installation 
=========
[![Build Status](https://travis-ci.com/gmarokov/ansible-playbook-postinstall-ubuntu.svg?branch=master)](https://travis-ci.com/gmarokov/ansible-playbook-postinstall-ubuntu)

Post Ubuntu installation Ansible script for provisioning dev machine.

## Installation
1. Install Ansible 
2. Add entry to your hosts in `/etc/ansible/hosts`:
```
[localhost] 
127.0.0.1
```

## Usage
`ansible-pull -U https://github.com/gmarokov/ansible-playbook-postinstall-ubuntu.git -e become-pass=your-sudo-pass`

## Script details 

### Pre tasks
- Update system

### Tasks

#### Install apt packages
- Git
- CopyQ
- Gnome Tweaks

#### Install snap packages
- Visual Studio Code
- Postman
- .NET Core SDK 2.1
- Node.js 12
- Docker
- Firefox
- Spotify
