[![Build Status](https://travis-ci.org/romanvbabenko/ansible-role-dockerbox.svg?branch=master)](https://travis-ci.org/romanvbabenko/ansible-role-dockerbox)

# Ansible Role: Dockerbox

Bootstrapping role for a new virtual machine box.
What it does ?
* install Docker CE
* install docker-compose
* configure passwordless sudoer user
* apply secure SSH config(disable root and regular user login with password, copy ssh key to server)
* enable UFW(Uncomplicated FireWall) and setup basic policies and allow ssh, http, and https

## Requirements

None.

## Role Variables

see [defaults/main.yml](defaults/main.yml)

## Dependencies

None.

## Example playbook

see [molecule/default/converge.yml](molecule/default/converge.yml)

## TODO

* fix idempotency when docker-compose version changing
* make the role more configurable, extract more variables

## License

MIT / BSD

Author Information

This role was created in 2020 by [Roman V. Babenko](https://romanvbabenko.github.io/)
