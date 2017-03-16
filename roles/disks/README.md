# disks

This role directory contains a collection of roles related to disks management
and filesystems.

# filesystem

This role creates the filesystems as specified by ```lvm_fs```.

# lvm

This role creates the Physical Volumes, Volume Groups, and Logical Volumes as
defined by ```lvm_pvs```, ```lvm_vgs```, and ```lvm_lvs```.

# mounts

This role will mount and update fstab as defined by ```lvm_mounts```.

# parted

This role will create the disk label and create one partition that spans the
entire disk. Disks altered are defined by ```lvm_pdisks```.

# Usage

There is one playbook that handles this all.

```
ansible-playbook -i /path/to/inventory disks.yml
```
