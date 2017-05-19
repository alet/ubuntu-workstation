# Ubuntu Workstation

This playbook configure typical workstation on Ubuntu

If you configure localhost you need install ansible & git before

```sh
sudo apt-get install ansible git
git clone git@github.com:alet/ubuntu-workstation.git
cd ubuntu-workstation
cat <<EOF > stage
[workstation]
localhost
EOF
ansible-playbook -b -K -i stage site.yml
```
