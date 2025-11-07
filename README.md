# Ansible Collection - johe37.k8s

Documentation for the collection.

## Install Kubernetes cluster

Currently only tested on Debian 12.

Create an ansible inventory under `inventory/cluster.yml`. Inventory sample
`inventory/cluster.yml.sample` exists for inspiration.

### Playbooks

```shell
# Pre-flight check
ansible-playbook playbooks/install-k8s-cluster.yml --tags=check

# Start the installation:
ansible-playbook playbooks/install-k8s-cluster.yml --skip-tags=check
```

