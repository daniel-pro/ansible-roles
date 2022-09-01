Role Name
=========

common-linux

Requirements
------------

Access the YUM repository to download the required packages


Role Variables
--------------

common_packages: a list of packages to be installed on the machine

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: common-linux }

License
-------

GNU General Public License v3.0


Author Information
------------------

Daniel Procopio https://github.com/daniel-pro
