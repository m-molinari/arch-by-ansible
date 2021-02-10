Role Name
=========

rsyslog 

Requirements
------------

- Ansible
- systemd

Dependencies
------------
roles/paru

Example Playbook
----------------

This example is a simple playbook called test.yml 

use: 
```yaml
ansible-playbook tests/test.yml --check --diff
```
to try this role

test.yaml :

```yaml
---
- name: test rsyslog module
  hosts: localhost
  become: yes

  roles:
    - rsyslog
```
