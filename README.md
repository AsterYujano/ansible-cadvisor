# ansible-cadvisor

Ansible module for [cadvisor](https://github.com/google/cadvisor)

## Getting started

1. Clone the repository in `roles/` folder

2. Add it to your playbook `metrics.yml`

```yml
---
- name: Install metrics
  hosts: metrics

  roles:
    - cadvisor

  vars:
    cadvisor_port: "9966"
```

3. Run it 

```bash
ansible-playbook -i ./hosts metrics.yml
```
