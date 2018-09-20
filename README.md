# Ubuntu Workstation

This playbook configure typical workstation on Ubuntu

If you configure localhost you need install ansible & git before. Ansible should be at least 2.1 so in 16.04 you need install it by pip

```sh
pip install --user ansible
sudo apt-get install git
git clone git@github.com:alet/ubuntu-workstation.git
cd ubuntu-workstation
ansible-playbook --ask-become-pass -bc local -i 'localhost,' site.yml
```
Note: textract will be installed in home directory
