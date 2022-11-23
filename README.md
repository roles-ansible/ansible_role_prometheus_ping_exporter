[![License](https://raw.githubusercontent.com/roles-ansible/ansible_role_prometheus_ping_exporter/main/.github/license.svg)](https://github.com/roles-ansible/ansible_role_prometheus_ping_exporter/blob/main/LICENSE)
[![Galaxy](https://github.com/roles-ansible/ansible_role_prometheus_ping_exporter/raw/main/.github/galaxy.svg)](https://galaxy.github.com/do1jlr/prometheus_ping_exporter)

# Ansible role prometheus ping exporter
Ansible role to install the prometheus node exporter from [github.com/czerwonk/ping_exporte](https://github.com/czerwonk/ping_exporter.git)

## Some variables
| value | default |
| --- | --- |
| ping_exporter__user | ``ping_exporter`` |
| ping_exporter__group | ``ping_exporter`` |
| ping_exporter__user_home | ``/var/lib/ping_exporter`` |
| ping_exporter__shell | ``/bin/false`` |
| ping_exporter__version | ``latest`` |
| ping_exporter__targets | `` []`` |
| ping_exporter__nameserver | ``9.9.9.9`` |
| ping_exporter__web_listen_address | ``:9427`` |
| submodules_versioncheck | ``false`` |


