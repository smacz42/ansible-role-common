# Ansible Role: `common`

## Description

These are tasks common to all of my roles, including:

* Installing extra programs such as:
    * vim
    * tmux
    * nmap
    * rsync
* Setting the MOTD
* Installing, configuring, and starting:
    * fail2ban
    * rsyslog
    * yum-cron

## Requirements

* RHEL only

## Role Variables

```yaml
variable: value # comment
```

## Tags

### Role-Specific tags:

* `common`
* `common_install`
* `common_config`

### Global tags:

* `install`
* `config`

## Dependencies

## Example Playbook

```yaml
- name: Roles in Common
  hosts: all
  gather_facts: true
  remote_user: root

  roles:
    - { role: common }
```

## License

MIT / BSD

## Author Information

This role was created in 2017 by [Andrew Cz](https://andrewcz.com), a student at The Ohio State University.
