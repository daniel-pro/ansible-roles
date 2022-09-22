Role Name
=========

Role to configure a secondary vnic on Linux VMs in OCI

Requirements
------------

None

Role Variables
--------------

``` enable_secondary_vnic ``` triggers all tasks in the role. By default is set to ```false``` set it to ```true```


Dependencies
------------

None

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - { role: oci-secondary-vnic }
```

License
-------

GNU General Public License v3.0

Author Information
------------------

Daniel Procopio https://github.com/daniel-pro
