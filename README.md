[![Build Status](https://travis-ci.org/inmotionhosting/ansible-role-postgresql.png?branch=master)](https://travis-ci.org/inmotionhosting/ansible-role-postgresql) [![GPL-3.0 License](https://img.shields.io/github/license/inmotionhosting/ansible-role-postgresql.svg?color=blue)](https://github.com/inmotionhosting/ansible-role-postgresql/blob/master/LICENSE) [![GitHub stars](https://img.shields.io/github/stars/inmotionhosting/ansible-role-postgresql.svg)](https://github.com/inmotionhosting/ansible-role-postgresql/stargazers)

# Ansible Role: PostgreSQL

Modular Ansible Role for deploying and configuring PostgreSQL

## Requirements

* CentOS 7.x or later
* Debian 9 or later
* Ubuntu 16.04 LTS or later

## Dependencies

None.

## Role Variables

Available variables are listed below with their default values (you can also see `defaults/main.yml`)

| Variable | Description |
| -------- | ----------- |
| postgres_package | Default: `postgresql-server`
| postgres_data_dir | Default: `/var/lib/pgsql/data`
| postgres_conf_dir | Default: `/var/lib/pgsql/data` (Same as postgres_data_dir)
| postgres_user | Default: `postgres`

## Example Playbook

```yaml
- hosts: www
  roles:
    - role: inmotionhosting.postgresql
```

## License

GPLv3

## Author Information

[InMotion Hosting](https://inmotionhosting.com)
