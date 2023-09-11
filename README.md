[![Ansible Galaxy](https://ansible.l3d.space/svg/l3d.prometheus_ping_exporter.svg)](https://galaxy.ansible.com/l3d/prometheus_ping_exporter)
[![BSD-3 Clause](https://ansible.l3d.space/svg/l3d.prometheus_ping_exporter_license.svg)](LICENSE)
[![Maintainance](https://ansible.l3d.space/svg/l3d.prometheus_ping_exporter_maintainance.svg)](https://ansible.l3d.space/#l3d.prometheus_ping_exporter)

# Ansible role prometheus ping exporter
Ansible role to install the prometheus node exporter from [github.com/czerwonk/ping_exporter](https://github.com/czerwonk/ping_exporter.git)

## Some variables
| value | default |
| --- | --- |
| `ping_exporter__targets` | `` []`` |
| `ping_exporter__user` | ``ping_exporter`` |
| `ping_exporter__group` | ``ping_exporter`` |
| `ping_exporter__user_home` | ``/var/lib/ping_exporter`` |
| `ping_exporter__shell` | ``/bin/false`` |
| `ping_exporter__version` | ``latest`` |
| `ping_exporter__nameserver` | ``9.9.9.9`` |
| `ping_exporter__web_listen_address` | ``:9427`` |
| `ping_exporter__filename` | *see defaults/main.yml* |
| `ping_exporter__dns` | *see defaults/main.yml* |
| `ping_exporter__ping` | *see defaults/main.yml* |
| `ping_exporter__options` | *see defaults/main.yml* |
| `submodules_versioncheck` | ``false`` |


Please define all your targets in the ``ping_exporter__targets`` array.

## Example Playbook
```yml
---
- name: Install ping exporter at example.com
  hosts: example.com
  roles:
    - {role: do1jlr.prometheus_ping_exporter, tags: etebase}
  vars:
    ping_exporter__targets:
      - host1.example.com
      - host2.example.com
      - ccc.de
```
