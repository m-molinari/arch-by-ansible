# Ansible playbook for configuring Debian and Archlinux desktop with (Cinnamon DE)
Collection of roles for configure Debian and Arch linux Desktop
by installing desktop tools (gtk) Cinnamon DE expecially for ArchLinux

adding some iptables roles :

- Set the policy for the INPUT chain to DROP
- Allow related and established connections
- Allow loopback

for Archlinux will be installed and configured "rsyslog" "NetworkManager" "cups-browsed.service"

some roles will be executing only if "ansible_distribution" is equal to ArchLinux or Debian (for the moment, LinuxMint will be added)

Apt and pacman roles will install:
- themes 
- desktop_utilities: like audacity,bleachbit,gnome-disk-utility,simple-scan etc ...
- accessories: like keepassxc, vim etc ...
- clients: firefox-esr, filezilla, thunderbird+enigmail
sys tools: binutils, dnsutils, terminator, whois, wget etc ...

