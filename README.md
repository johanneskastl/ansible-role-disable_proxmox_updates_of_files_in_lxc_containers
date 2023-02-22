![Ansible Lint](https://github.com/johanneskastl/ansible-role-disable_proxmox_updates_of_files_in_lxc_containers/workflows/Ansible%20Lint/badge.svg)

disable_proxmox_updates_of_files_in_lxc_containers
=========

Disable modification of etc files inside LXC containers, done by Proxmox by default.

Requirements
------------

None.

Role Variables
--------------

None.

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: 'johanneskastl.disable_proxmox_updates_of_files_in_lxc_containers'

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
