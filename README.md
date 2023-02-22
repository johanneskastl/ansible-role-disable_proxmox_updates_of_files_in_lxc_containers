![Ansible Lint](https://github.com/johanneskastl/ansible-role-disable_proxmox_updates_of_files_in_lxc_containers/workflows/Ansible%20Lint/badge.svg)

disable_proxmox_updates_of_files_in_lxc_containers
=========

Disable modification of etc files inside LXC containers, done by [Proxmox by default](https://pve.proxmox.com/wiki/Linux_Container#_guest_operating_system_configuration).

Requirements
------------

This role is meant to be used on the LXC container, that is running on Proxmox. Do not use this role on the Proxmox host(s).

Role Variables
--------------

By default, the role will prohibit Proxmox from messing with `/etc/hosts` and `/etc/hostname` inside the container. If you want to allow one or the other, set the following variables accordingly:

- `disable_etc_hosts_modification`: (Boolean) If you want to allow Proxmox to modify `/etc/hosts`, set this to `false`. Default value is `true`.
- `disable_etc_hostname_modification`: (Boolean) If you want to allow Proxmox to modify `/etc/hostname`, set this to `false`. Default value is `true`.

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
