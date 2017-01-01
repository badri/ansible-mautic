# README.md
# Ansible Role: mats116.composer

An Ansible role that installs composer on **Ubuntu 14.04 LTS**

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

```yaml
composer_install_dir: /usr/local/composer
composer_bin_location: /usr/local/bin/composer
```

## Dependencies

none

## Example Playbook

```yaml
- hosts: web-server
  roles:
    - role: mats116.composer
```

## License

MIT
