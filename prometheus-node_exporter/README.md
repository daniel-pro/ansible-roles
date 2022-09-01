Role Name
=========

Prometheus node exporter installation role

Requirements
------------

Access to github for downloading the package.


Role Variables
--------------

node_exporter_version: the version of the node exporter to be installed
node_exporter_arch: the architecture of the binary to be installed
node_exporter_download_url: the URL from which we can download the packaged exporter
node_exporter_bin_path: the path on the local system where the exporter will be installed in
node_exporter_options: the options to pass to the node exporter
node_exporter_state: the desired state of the exporter
node_exporter_enabled: whether the exporter is enabled or not


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: prometheus-node_exporter }

License
-------

GNU General Public License v3.0

Author Information
------------------

Daniel Procopio https://github.com/daniel-pro
