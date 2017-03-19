# homelab-kubernetes

Ansible project for building out a simple Kubernetes cluster from scratch.

# Usage

Note: The server that is executing the playbooks needs to be within the
environment. These playbooks are not designed to handle floating IPs.

* Set up your AWS environment (3x masters, 3x nodes)
  * AMI: CentOS 7 - x86-64 with HVM (although any other RHEL/CentOS/Fedora
  based distribution should work)
* ```git clone https://github.com/digaxfr/homelab-kubernetes.git```
* Configure ```homelab-kubernetes/hosts```
* ```ansible-playbook -i hosts deploy.yml```

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
| ipv6          | Manual notes |

## Container Networking

While I have work experience with Calico, I have decided to start off with
flannel first because it is simple for this project and something new to learn.
After the initial set of playbooks are complete, I will look to implement a
Calico based solution.

# License

MIT
