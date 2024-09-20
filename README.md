Proxmox_Templates_Delete
=========

The task delete template vmid in Proxmox

Requirements
------------

Proxmox 8.2.4+\
ansible 3.1.2+\
ansible-galaxy 2.16.11+\
Not tested on earlier versions

Role Variables
--------------

___proxmox_api_host:___ "127.0.0.1"\
___proxmox_api_user:___ "root@pam"\
___proxmox_api_password:___ "password"\
___proxmox_node:___ "pve"\
___vmid:___ 100 - ID template in proxmox

Dependencies
------------

Dependencies are absent

Example Playbook
----------------

```
- name: Delete templates in Proxmox
  hosts: proxmox
  vars:
    proxmox_api_host: "proxmox1.home.local"
    proxmox_api_user: "root@pam"
    proxmox_api_password: "11111111"
    proxmox_node: "proxmox1" 
    vmid: "9004"
  roles:
    - Proxmox_Templates_Delete
```

License
-------

BSD-3-Clause

Author Information
------------------

Murzabaev Marat (murzik2142@gmail.com)
