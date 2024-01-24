# Ubuntu Workstation

This playbook configure typical workstation on Ubuntu

If you configure localhost you need install ansible & git before. Ansible should be at least 2.1 so in 16.04 you need install it by pip

You may want change default values for example for golang (roles/golang/default/main.yml)

```sh
sudo apt-get install git ansible python3-pip
ansible-galaxy collection install community.general
git clone https://github.com/alet/ubuntu-workstation.git/
cd ubuntu-workstation
ansible-playbook --ask-become-pass -c local -i 'SHORT_HOSTNAME,' site.yml
```
Notes:
- textract will be installed in home directory
- There was issue with nmcli module (make bridge in virt role): https://github.com/ansible/ansible/pull/58115
- Telegram should be installed in .local due to update schema
