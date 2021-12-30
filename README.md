# Ansible playbook for configure Arch Linux OS
Collection of roles for configure Arch linux with Cinnamon DE and a complete Desktop and utilities
You have to use "startx" command for starting desktop env

Note:
you must change change_me with your user in this file :
https://github.com/m-molinari/arch-by-ansible/blob/master/group_vars/all

You can find basic initial installation commands for Arch Linux here:
https://gist.github.com/m-molinari/be93633337110b529cff38f1aab96e66

# Requirements
Ansible is a must! Some roled need fakeroot

# Desktop or Window manager
You can choice if installing cinnamon desktop or i3wm by comment and uncomment in playbook roles
by default cinnamon will be installed :

```
  - cinnamon
  #- i3wm
```  
 
 # Roles
 
| Role                    | Required | Default | Dependences       | Comments                                        |
| ----------------------- | -------- | ------- | ----------------- | ----------------------------------------------- |
| config                  | yes      | true    | ansible           | LoveCandy, wifi config, noobeep in terminal     |
| iptables                | yes      | true    | ansible           | config firewall                                 |
| pacman                  | yes      | true    | ansible           | Installing packages                             |
| yay                     | yes      | true    | ansible, fakeroot | Installing yay and some packages                |
| services                | yes      | true    | ansible           | config services (NetworkManager, cups ecc ...)  | 
| rsyslog                 | yes      | true    | ansible, fakeroot | Installing and config syslog                    |
| cinnamo                 | yes      | true    | ansible           | Installing DE Cinnamon                          |
| i3wm                    | yes      | false   | ansible           | Installing WM i3wm                              |

Install dependences in Archlinux
```
sudo pacman -S ansible fakeroot
```
