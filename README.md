# Ansible Prometheus Node Exporter Role

[![Lint Ansible roles](https://github.com/francomile/ansible-role-prom-node-exporter/actions/workflows/ansible_lint.yml/badge.svg)](https://github.com/francomile/ansible-role-prom-node-exporter/actions/workflows/ansible_lint.yml)

[![Release role to Ansible Galaxy](https://github.com/francomile/ansible-role-prom-node-exporter/actions/workflows/push_to_galaxy.yml/badge.svg)](https://github.com/francomile/ansible-role-prom-node-exporter/actions/workflows/push_to_galaxy.yml)

## Actions of the Role

* Install Prometheus node_exporter

## Common Usage

```yaml
roles:
  - {
    role: francomile.prom-node-exporter,
    prom_node_exporter_basedir: "/opt/node_exporter",
    prom_node_exporter_version: "v1.8.1",
    tags: ["node-exporter"]
  }
```

## Run the playbook

```shell
ansible-playbook -i inventory playbook.yaml -t "node-exporter"
```
