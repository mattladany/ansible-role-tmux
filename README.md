Ansible Role - Tmux
=========

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://raw.githubusercontent.com/mattladany/ansible-role-tmux/master/LICENSE)

Installs [tmux](https://github.com/tmux/tmux) from source on RedHat/Centos, Debian/Ubuntu or MacOS systems.

Requirements
------------

Requirements can be installed manually by the user or through the role by setting ```tmux_install_requirements: yes```.

The Requirements are:

- A working C compiler (e.g., gcc)
- make
- autoconf
- automake
- pkg-config
- libevent
- ncurses

This list of requirements was taken directly from the tmux [README](https://raw.githubusercontent.com/tmux/tmux/master/README) so I am assuming it is correct and complete.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

None.

Example Playbook
----------------

```
- hosts: servers
  roles:
     - { role: mattladany.tmux, tmux_version: 2.8, tmux_install_requirements: yes }
 ```

License
-------

MIT

Author Information
------------------

This role was created and is maintained by Matt Ladany.
