# docker

This role will install docker engine and configure itself to work with the etcd
cluster and integrate with into flannel.

Currently this role configures docker options completely on CLI arguments.

# Dependencies

* ```/var/lib/docker``` volume should be formatted correctly (xfs, ftype=1)
and mounted

# Usage

```
ansible-playbook -i /path/to/inventory docker.yml
```
