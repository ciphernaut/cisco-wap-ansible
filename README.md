



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
```


