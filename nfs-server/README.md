Role Name
=========

This role installs all required packages and configures the nfs server on Oracle Linux servers.

Requirements
------------

None

Role Variables
--------------

``` nfs_rpcbind_state ```:  should be always "started"
``` nfs_rpcbind_enabled ```: should always be "true"
``` nfs_exports ```: defines the directories to be exported to which clients. 


```
nfs_rpcbind_state: started
nfs_rpcbind_enabled: true
nfs_exports:
  - path: "/dir1"
    access:
      - clients: "*"
        options: "(rw,sync,no_root_squash)"
```

Dependencies
------------

None

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - { role: nfs-server }
```

License
-------

GNU General Public License v3.0


Author Information
------------------

Daniel Procopio https://github.com/daniel-pro