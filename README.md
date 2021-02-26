# Ansible Role - Tmux

[![CI](https://github.com/geerlingguy/ansible-role-ntp/workflows/CI/badge.svg?event=push)](https://github.com/mattladany/ansible-role-tmux/actions?query=workflow%3ACI)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](https://raw.githubusercontent.com/mattladany/ansible-role-tmux/master/LICENSE)

Installs [tmux](https://github.com/tmux/tmux/wiki) from source on Centos and Debian systems.

## Requirements

- A working C compiler (e.g., gcc)
- make
- autoconf
- automake
- pkg-config
- libevent
- ncurses

This list of requirements is taken directly from the tmux [README](https://raw.githubusercontent.com/tmux/tmux/master/README) so it is assumed to be correct and complete.

## Role Variables

Available variables are listed below, along with their default values (see ```defaults/main.yml```):

```tmux_version: 3.1```

Set this to the version of tmux you would like to install. See [here](https://github.com/tmux/tmux/releases) for a list of tmux releases.

```tmux_download_dir```

Where to download and unarchive the tmux tarball to.

```tmux_download_url```

The URL of which the tarball should be downloaded from.

## Dependencies

None.

## Example Playbook

```
- hosts: servers
  roles:
    - { role: mattladany.tmux }
 ```

## License

[MIT](https://raw.githubusercontent.com/mattladany/ansible-role-tmux/master/LICENSE)

## Author Information

This role was created by Matt Ladany.
