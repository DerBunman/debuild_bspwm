# ansible role debuild_bspwm
Ansible cookbook to build and install a bspwm .deb for Ubuntu/Debian.

# example
## playbook.yml
I install bspwm on all hosts in the desktop group.
```yaml
- hosts: desktop
  roles:
    - derbunman.debuild_bspwm
```

## requirements.yml
```yaml
- src: derbunman.debuild
- src: derbunman.debuild_bspwm
```

## install dependencies
```sh
ansible-galaxy install -r requirements.yml
```

## update dependencies
```sh
ansible-galaxy install -r requirements.yml --force
```

## run playbook
```sh
ansible-playbook playbook.yml -v
```
