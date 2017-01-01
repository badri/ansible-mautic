# README.md
# Ansible Role: mats116.mautic

An Ansible role that installs [mautic](https://www.mautic.org/) on **Ubuntu 14.04 LTS**

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

```yaml
mautic_version: "1.2.2"

mautic_nginx_accesslog: /var/log/nginx/mautic-access.log

mautic_mysql_host: localhost
mautic_mysql_database: mautic
mautic_mysql_user: mautic
mautic_mysql_password: mautic

composer_github_token:
```

## Dependencies

- [mats116.nginx](https://galaxy.ansible.com/detail#/role/6198) - Installer of Nginx
- [mats116.php5-fpm](https://galaxy.ansible.com/detail#/role/6238) - Installer of php-fpm
- [mats116.mariadb-server](https://galaxy.ansible.com/detail#/role/6199) - Installer of MariaDB Server (MySQL)
 - `when "mautic_mysql_host == 'localhost'"`

## Example Playbook

```yaml
- hosts: mautic-server
  roles:
    - role: mats116.mautic
      composer_github_token: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

## License

MIT
