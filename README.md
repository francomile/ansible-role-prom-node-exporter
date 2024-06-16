# Ansible Prometheus Node Exporter Role

## Actions of the Role

* Install Prometheus node_exporter

## Common Usage

```yaml
roles:
  - {
    role: prom_node_exporter,
    prom_node_exporter_basedir: "/opt/node_exporter",
    prom_node_exporter_version: "v1.8.1",
    tags: ["node-exporter"]
  }
```

## Run the playbook

```shell
ansible-playbook -i inventory playbook.yaml -t "node-exporter"
```
