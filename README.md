ansible-role-fedora-base
=========

[![Build Status](https://travis-ci.org/lborguetti/ansible-role-fedora-base.svg?branch=master)](https://travis-ci.org/lborguetti/ansible-role-fedora-base)

This role install the common packages I used by Fedora bootstrap.

Requirements
------------

Ansible itself.

Role Variables
--------------

- `dns_servers`: List with the dns servers.
- `packages_common`: List with the common packages to install.
- `inbound_tcp_ports`: List with the tcp ports to allow inbound traffic.
- `outbound_tcp_ports`: List with the tcp ports to allow outbound traffic.
- `outbound_udp_ports`: List with the udp ports to allow outbound traffic.
- `private_networks`: List with the private networks to allow unprivileged ports traffic.

See the values in the vars files.

Role Tags
---------

- `packages`: run only packages tasks.
- `iptables`: run only iptables tasks.


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ansible-role-fedora-base }

License
-------

MIT

Author Information
------------------

Luciano Antonio Borguetti Faustino
