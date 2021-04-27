# jtprogru.install_base_soft

![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jtprogru/ansible-role-install-base-soft/CI?label=CI)
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jtprogru/ansible-role-install-base-soft/Release?label=Release)
![GitHub](https://img.shields.io/github/license/jtprogru/ansible-role-install-base-soft)
[![Ansible Role](https://img.shields.io/ansible/role/53229)](https://galaxy.ansible.com/jtprogru/ansible-role-install-base-soft/)
[![GitHub tag](https://img.shields.io/github/tag/jtprogru/ansible-role-install-base-soft.svg)](https://github.com/jtprogru/ansible-role-install-base-soft/tags)

Simple role for install base soft for comfort using remote server.


## Role Variables


See [`defaults/main.yml`](defaults/main.yml).


## Example Playbook

Example playbook:
```yaml
---
- name: Installing basic software
  hosts: all
  become: true

  vars:
    base_soft_list_extra:
      - ansible
      - net-tools
      - python3-pip
      - python3-setuptools
      - python3-wheel
      - ansible-lint
      - yamllint

  roles:
    - jtprogru.install_base_soft
```

## License

See [LICENSE](LICENSE.md)
