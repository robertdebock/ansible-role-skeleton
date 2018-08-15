{{ cookiecutter.role_name }}
=========

[![Build Status](https://travis-ci.org/robertdebock/ansible-role-{{ cookiecutter.role_name}}.svg?branch=master)](https://travis-ci.org/robertdebock/ansible-role-{{ cookiecutter.role_name}})

Provides {{ cookiecutter.role_name }} for your system.

Context
--------
This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://robertdebock.nl/) for further information.

Here is an overview of related roles:
![dependencies](https://raw.githubusercontent.com/robertdebock/drawings/artifacts/{{ cookiecutter.role_name }}.png "Dependency")

Requirements
------------

- Access to a repository containing packages, likely on the internet.
- Ansible 2.2 or higher. (Tests run on the last 3 release of Ansible.)

Role Variables
--------------

- {{ cookiecutter.role_name }}_parameter: Description of values. [default: value]

Dependencies
------------

- None known.

Compatibility
-------------

This role has been tested against the following distributions and Ansible version:

|distribution|ansible 2.4|ansible 2.5|ansible 2.6|
|------------|-----------|-----------|-----------|
|alpine-edge|yes|yes|yes|
|alpine-latest|yes|yes|yes|
|archlinux|yes|yes|yes|
|centos-6|yes|yes|yes|
|centos-latest|yes|yes|yes|
|debian-latest|yes|yes|yes|
|debian-stable|yes|yes|yes|
|fedora-latest|yes|yes|yes|
|fedora-rawhide|yes|yes|yes|
|opensuse-leap|yes|yes|yes|
|opensuse-tumbleweed|yes|yes|yes|
|ubuntu-artful|yes|yes|yes|
|ubuntu-latest|yes|yes|yes|

Example Playbook
----------------

```
---
- name: {{ cookiecutter.role_name }}
  hosts: all
  gather_facts: no
  become: yes

  roles:
    - role: robertdebock.{{ cookiecutter.role_name }}

```

To install this role:
- Install this role individually using `ansible-galaxy install robertdebock.{{ cookiecutter.role_name }}`

Sample roles/requirements.yml: (install with `ansible-galaxy install -r roles/requirements.yml
```
---
- name: robertdebock.bootstrap
```

License
-------

Apache License, Version 2.0

Author Information
------------------

[Robert de Bock](https://robertdebock.nl/) <robert@meinit.nl>
