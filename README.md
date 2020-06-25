# Ansible Role: resolvers

Simple role that manages resolv.conf automatically on RedHat/CentOS, Debian and Ubuntu-based systems.

## Requirements

None

## Installation

`ansible-galaxy install vdzhorov.resolvers`

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    resolv_conf_nameservers: []

The `resolv_conf_nameservers` list is not mandatory, it will be set up from role defaults. You can however set it to whatever you'd like in your group_vars/host_vars in order to override it.

## Dependencies

None

## Example Playbook

    - hosts: all
      roles:
        - vdzhorov.resolvers

## License

MIT
