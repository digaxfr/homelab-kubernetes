# ca_trust

This role adds the custom CA root into trusted CA store. This role is targeted
for RHEL/CentOS/Fedora based distributions.

# Dependencies

The following variables need to be defined:

| Variable | Content |
|--------------------|
| certs_ca | The CA certificate file |

# Usage

```
ansible-playbook -i /path/to/inventory ca_trust.yml
```
