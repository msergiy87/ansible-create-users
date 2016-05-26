# ansible-create-users

Create on each server (file hosts) users from the list (file users.yml).

User Settings
------------

- Shell = /bin/bash
- Add the public key from pub_keys dir
- In users.yml specify that user should have the right to sudo or not

Distros tested
------------

Currently, this is only tested on Centos 6.7 as a client machine and Ubuntu 14.04 as a server machime.

Usage
------------

```
ansible-playbook -i hosts create_users.yml
```
