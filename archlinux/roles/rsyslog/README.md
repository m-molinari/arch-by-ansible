Role Name
=========

rsyslog 

Requirements
------------

- Ansible
- systemd

Dependencies
------------
roles/yay

Example Playbook
----------------

This example is a simple playbook.yml 

use: ansible-playbook tests/test.yml --check --diff
to try this role

---
- name: test rsyslog module
  hosts: localhost
  become: yes

  roles:
    - rsyslog

