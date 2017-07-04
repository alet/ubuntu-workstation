# Ubuntu Workstation

[![Build Status](https://travis-ci.org/alet/ubuntu-workstation.svg?branch=master)](https://travis-ci.org/alet/ubuntu-workstation)

This playbook configure typical workstation on Ubuntu

If you configure localhost you need install ansible & git before

```sh
sudo apt-get install ansible git
git clone git@github.com:alet/ubuntu-workstation.git
cd ubuntu-workstation
ansible-playbook --ask-become-pass -bc local -i 'localhost,' site.yml
```
