# yum

This directory contains a collection of roles relating to th eyum package
manager.

# upgrade

This role performs a ```yum upgrade``` and reboots the target node. A
```wait_for``` is implemented to ensure that connection can be established
again.

## usage

```
ansible-playbook -i /path/to/inventory yum_upgrade.yml
```
