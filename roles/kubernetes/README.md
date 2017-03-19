# kubernetes

This directory contains a collection of roles related to deploying Kubernetes.

# bootstrap_files

This role is responsible for grabbing the initial tarball package as specified
by various variables set in ```group_vars/all/kubernetes.yml```.

# bootstrap_files_remote

This role is responsible for pushing out the necssary tarball packages out to
the endpoint nodes.
