Role Name
=========
iptables 

This role configure iptables to DROP INPUT connection by default
ACCEPT related, established
ACCEPT all from loopback interface
Manages rules saved on /etc/iptables/iptables.rules via iptables-save

Requirements
------------
* Ansible
* Iptables

