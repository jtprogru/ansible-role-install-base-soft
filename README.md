# jtprog.install_base_soft

![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jtprog/ansible-role-install-base-soft/CI?label=CI) ![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jtprog/ansible-role-install-base-soft/Release?label=Release) ![GitHub](https://img.shields.io/github/license/jtprog/ansible-role-install-base-soft)

Simple role for install base soft for comfort using remote server.


## Role Variables


A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.


## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
---
- name: Installing basic software
  hosts: all
  become: true

  vars:
    base_soft_list_extra:
      - { name: ansible, state: latest }
      - { name: net-tools, state: latest }
      - { name: python3-pip, state: latest }
      - { name: python3-setuptools, state: latest }
      - { name: python3-wheel, state: latest }
      - { name: ansible-lint, state: latest }
      - { name: yamllint, state: latest }

  roles:
    - jtprog.install_base_soft
```

## License

[WTFPL](LICENSE.md)
