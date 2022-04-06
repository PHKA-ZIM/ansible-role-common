# Installation helper for ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-installer
  name: ansible-role-installer
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-installer

- Import role and override role variables, e.g.
```
- name: Install repositories and packages
  roles:
    - role: ansible-role-installer
```
