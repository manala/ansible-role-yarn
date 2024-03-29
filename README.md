#######################################################################################################

# :exclamation: DEPRECATION :exclamation:

## This repository and the role associated are deprecated in favor of the [Manala Ansible Collection](https://galaxy.ansible.com/manala/roles)

## You will find informations on its usage on the [collection repository](https://github.com/manala/ansible-roles)

#######################################################################################################

# Ansible Role: Yarn [![Build Status](https://travis-ci.org/manala/ansible-role-yarn.svg?branch=master)](https://travis-ci.org/manala/ansible-role-yarn)

:exclamation: [Report issues](https://github.com/manala/ansible-roles/issues) and [send Pull Requests](https://github.com/manala/ansible-roles/pulls) in the [main Ansible Role repository](https://github.com/manala/ansible-roles) :exclamation:

This role will deal with the setup of [Yarn](https://yarnpkg.com/).

It's part of the [Manala Ansible stack](http://www.manala.io) but can be used as a stand alone component.

## Requirements

None.

## Dependencies

None.

## Installation

### Ansible 2+

Using ansible galaxy cli:

```bash
ansible-galaxy install manala.yarn
```

Using ansible galaxy requirements file:

```yaml
- src: manala.yarn
```

## Role Variables

### Definition

| Name                                   | Default  | Type  | Description                            |
| -------------------------------------- | -------- | ----- | -------------------------------------- |
| `manala_yarn_install_packages`         | ~        | Array | Dependency packages to install         |
| `manala_yarn_install_packages_default` | ['yarn'] | Array | Default dependency packages to install |

## Example playbook

```yaml
- hosts: servers
  roles:
    - { role: manala.yarn }
```

# Licence

MIT

# Author information

Manala [**(http://www.manala.io/)**](http://www.manala.io)
