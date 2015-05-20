cassandra
=========

Installs and configures Apache Cassandra

Requirements
------------

This role requires Ansible 1.4 or higher.

Role Variables
--------------

| Name              | Default | Description                     |
|-------------------|---------|---------------------------------|
| cassandra_version | 2.1.5   | Version of Cassandra to install |

Dependencies
------------

- kbrebanov.java (OpenJDK 8)

Example Playbook
----------------

Install Cassandra
```
- hosts: all
  roles:
    - { role: kbrebanov.cassandra }
```

Install earlier version of Cassandra
```
- hosts: all
  roles:
    - { role: kbrebanov.cassandra, cassandra_version: 2.0.15 }
```

License
-------

BSD

Author Information
------------------

Kevin Brebanov
