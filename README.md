Ansible playbook: Post Ubuntu workstation installation 
=========
[![Build Status](https://travis-ci.org/gmarokov/ansible-playbook-postinstall-fedora.svg?branch=master)](https://travis-ci.org/gmarokov/ansible-playbook-postinstall-fedora)
Post Ubuntu installation Ansible script for provisioning dev machine.

## Installation
1. Install Ansible 
2. Add `[localhost] 127.0.0.1` to your hosts in /etc/ansible/hosts

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
- Firefox
- Docker
- Spotify
