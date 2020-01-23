Role Name
=========
iptables 

This role configure iptables to DROP INPUT connection by default
ACCEPT related, established
ACCEPT all from loopback interface
Enable iptables.service that manages rules saved on /etc/iptables/iptables.rules
by iptables-save

Requirements
------------
* Ansible
* Iptables

