



setup
=====

a file not included in this repo contains these variables:
inventory/group_vars/ios.yml

```
ansible_connection: network_cli
ansible_network_os: ios
ansible_user_a: ansible
ansible_user: "{{ ansible_user_a }}"
ansible_password_a: # some securely set password for the ansible user
ansible_password: "{{ ansible_password_a }}"
ansible_become: yes
ansible_become_password_a:   # some securely set enable password
ansible_become_password: "{{ ansible_become_password_a }}"
ssid_password|ciscohash7: password for SSID.  used with ciscohash7 function from
ansible-filter-cisco-hash repo
ssid_ssid_name:  SSID name top operate on
```


python modules
==============

from python3, OS distribution preferred
passlib
packaging


additional roles
================

ansible-galaxy -p ./playbooks/ap/roles/  install -f git+https://github.com/mjuenema/ansible-filter-cisco-hash.git


note
====

additional python modules and roles needed for password and ssid key hashing
functions

