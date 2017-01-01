# README.md
# Ansible Role: mats116.mariadb-server

An Ansible role that installs MariaDB Server on **Ubuntu 14.04 LTS**

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

    mariadb_version: "10.1"

    mariadb_root_password: root

## Dependencies

none

## Example Playbook

    - hosts: db-server
      roles:
        - role: mats116.mariadb-server
          mariadb_root_password: 12345678

## License

MIT
