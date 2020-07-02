inmotionhosting.postgresql
=======

Modular Ansible Role for deploying and configuring PostgreSQL

[![Build Status](https://travis-ci.org/inmotionhosting/ansible-role-postgresql.png?branch=master)](https://travis-ci.org/inmotionhosting/ansible-role-postgresql)


Requirements
------------

* CentOS 7.x or later
* Debian 8 or later
* Ubuntu 16.04.x LTS or later

Role Variables
--------------

| Variable | Description |
| -------- | ----------- |
| postgres_package | Default: `postgresql-server`
| postgres_data_dir | Default: `/var/lib/pgsql/data`
| postgres_conf_dir | Default: `/var/lib/pgsql/data` (Same as postgres_data_dir)
| postgres_user | Default: `postgres`

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: www
      roles:
         - role: inmotionhosting.postgresql

License
-------

GPLv3

Author Information
------------------

[InMotion Hosting](https://inmotionhosting.com)
