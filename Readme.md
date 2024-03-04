# Readme

## How to use it

In order to launch the `rice.yml` playbook.

```sh
ansible-playbook -i hosts rice.yml --ask-become-pass
example ansible-playbook --extra-vars="ansible_python_interpreter=$(which python)" -i hosts rice.yml --ask-become-pass --tags gnome-terminal -v
```

## Good links

https://github.com/briandipalma/ansible/tree/main


## Dumping gnome terminal options

```sh
$ dconf dump /org/gnome/terminal/legacy/profiles:/ > gnome-terminal-profiles.dconf
$ dconf load /org/gnome/terminal/legacy/profiles:/ < gnome-terminal-profiles.dconf
```