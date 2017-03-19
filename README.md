# homelab-kubernetes

Ansible project for building out a simple Kubernetes cluster from scratch.

# Progression

Note that these topics are high-level topics. They do not represent the actual
ansible roles.

| Topic         | Status       |
|---------------|--------------|
| aws bootstrap | Not started  |
| etcd          | Ansible done |
| flannel       | Ansible done |
| calico        | Not started  |
| docker        | Ansible done |
| kubernetes    | Manual notes |

## Container Networking

While I have work experience with Calico, I have decided to start off with
flannel first because it is simple for this project and something new to learn.
After the initial set of playbooks are complete, I will look to implement a
Calico based solution.

# License

MIT
