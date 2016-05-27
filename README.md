# ansible-create-users

Create on each server (file hosts) users from the list (file users.yml).

![ansible-create-users](https://github.com/msergiy87/ansible-create-users/blob/master/ansible-create-users.jpg)

User Settings
------------

- Shell = /bin/bash
- Add the public key in pub_keys dir (username.pub)
- In users.yml specify that user should have the right to sudo or not

Distros tested
------------

Currently, this is only tested on Ubuntu 14.04 as a client and server machine. It should theoretically work on older versions of Ubuntu or Debian based systems.

Usage
------------
- install ansible
- create keys
- configure client server authorized_keys
- upload repository and change
- run command

```
ansible-playbook -i hosts create_users.yml
```
