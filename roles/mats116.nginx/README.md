# README.md
# Ansible Role: mats116.nginx

An Ansible role that installs Nginx on **Ubuntu 14.04 LTS**

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

    nginx_version: ""

    nginx_user: nginx
    nginx_error_log_file: /var/log/nginx/error.log
    nginx_error_log_level: warn
    nginx_pid: /var/run/nginx.pid

    nginx_worker_processes: auto
    nginx_worker_rlimit_nofile: 4096
    nginx_worker_connections: 1024

    nginx_keepalive_timeout: 180

    logrotate_file: "/var/log/nginx/*.log"
    logrotate_period: 10


## Dependencies

none

## Example Playbook

    - hosts: web-server
      roles:
        - role: mats116.nginx
          nginx_version: "1.9.5"

## License

MIT
