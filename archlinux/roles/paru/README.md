Role Name
=========

Simple role for installing Paru helper for managing AUR packages

took a lot of inspiration from https://github.com/lgaggini/ansible-arch/blob/master/roles/archcore

- You can define a list of packages in vars/main.yaml to adapt role to your needs , ex I added arch-silence-grub-theme-git and audio-recorder
```bash
list_of_packages:
    - arch-silence-grub-theme-git
    - audio-recorder
- You must change user attributes (name and home path) in vars/main.yaml :
```bash
user:
  name: you
  home: /home/you


