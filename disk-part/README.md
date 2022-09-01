Role Name
=========

This role manages partitions, filesystems, entries in /etc/fstab and mounts all created filesystems.

Requirements
------------

None

Role Variables
--------------

Example:

```
disks:
  - dev_name: sdb
    label: gpt
    fs_type: xfs
    mount_point: /data
    mount_opts: defaults
  - dev_name: sdc
    label: msdos
    fs_type: xfs
    mount_point: /data2
    mount_opts: defaults    
```

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: disk-part }

License
-------

GNU General Public License v3.0

Author Information
------------------

Daniel Procopio https://github.com/daniel-pro
