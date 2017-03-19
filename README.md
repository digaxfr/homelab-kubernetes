# homelab-kubernetes

Ansible project for building out a simple Kubernetes cluster from scratch.

# Progression

| Topic         | Status       |
|---------------|--------------|
| aws bootstrap | Not started  |
| etcd          | Ansible done |
| flannel       | Manual notes |
| calico        | Not started  |
| docker        | Manual notes |
| kubernetes    | Manual notes |

## Container Networking

While I have work experience with Calico, I have decided to start off with
flannel first because it is simple for this project and something new to learn.
After the initial set of playbooks are complete, I will look to implement a
Calico based solution.

# License

MIT
