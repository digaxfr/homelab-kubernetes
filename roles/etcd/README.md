# etcd

This directory contains a collection of roles related to etcd.

# new_cluster

The ```etcd/new_cluster``` role deploys a new etcd cluster. The target hosts
are controlled by the hostgroup ```etcd_cluster```.

Note that this role is specific for only bringing a new cluster online.

## Certificates

etcd will be configured in a (somewhat) secure fashion using TLS. Client
communication and peer communication will transmit over TLS and will also be
authenticated by TLS certifcates.

The certificates being used need to both support TLS Client Authentication and
TLS Server Authentication.

## Dependencies

The following variables must be defined:

| Variable | Description |
|----------|-------------|
| etcd_ca | The CA certificate for the etcd cluster |
| etcd_cert | The server certificate for the etcd cluster |
| etcd_key | The server private key for the etcd cluster |

## Usage

```
ansible-playbook -i /path/to/inventory etcd_new_cluster.yml
```
