# Intro

🚧 This is a dev cluster setup automation, with Ansible, for spinning up a local development environment from the ground up.

# Requirements

kind:
`ansible-galaxy collection install community.kubernetes`

# Usage

## Install all

```bash
sudo ansible-playbook dapr-local-cluster.yml --tags "create, dapr-install, redis-install, zipkin-install, dapr-components-install"
```
