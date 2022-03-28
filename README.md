# Common setup automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-common
  name: ansible-role-common
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-common

- Import role and override role variables, e.g.
```
- name: Setup common
  roles:
    - role: ansible-role-common
```
