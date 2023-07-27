# Intro

🚧 This is a dev cluster setup automation, with Ansible, for spinning up a local development environment from the ground up.

# Requirements

- kind
- helm
- ansible
- tilt
- ctlptl

## Ansible modules
```bash
ansible-galaxy collection install community.kubernetes
```

## Helm repositories

```bash
helm repo add bitnami https://charts.bitnami.com/bitnami
```

# Usage

## Install all

```bash
ansible-playbook dapr-local-cluster.yml --tags "create, dapr-install, redis-install, zipkin-install, dapr-components-install"
```
