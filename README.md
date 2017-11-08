Ansible LAMP example with vagrant + Debian Jessie

Base package installation (no config) of nginx > apache > mysql

Set ansible hosts config file to match vagrant box ports and key paths.

Check connectivity:
ansible web,lb,db -i hosts -m ping

Run playbook:
ansible-playbook -i hosts lamp.yml
