# README.md
# Ansible Role: mats116.php5-fpm

An Ansible role that installs php5-fpm on **Ubuntu 14.04 LTS**

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

```yaml
php_version: "5.5"

# Resource Limits
max_execution_time: 30
max_input_time: 60
memory_limit: 128M

# Data Handling
post_max_size: 8M
always_populate_raw_post_data: 0

# Module Settings
date_timezone: Asia/Tokyo
```

## Dependencies

none

## Example Playbook

```yaml
- hosts: web-server
  roles:
    - role: mats116.php5-fpm
      php_version: "5.6"
```

## License

MIT
