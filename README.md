# Webarchitects Ansible Composer Role

[![pipeline status](https://git.coop/webarch/composer/badges/master/pipeline.svg)](https://git.coop/webarch/composer/-/commits/master)

An ansible role for Debian and Ubuntu which downloads installs [Composer](https://getcomposer.org/) globally to `/usr/local/bin/composer`.

## Role variables

Set `composer` to `true` for the tasks in this role to be run.

Documentation for the [defaults/main.yml](defaults/main.yml) variables follow, this documentation has been generated from the [meta/argument_specs.yml](meta/argument_specs.yml).

### Entrypoint: main

The main entry point for the composer role.

|Option|Description|Type|Required|
|---|---|---|---|
| composer | Run the tasks in this role. | bool | yes |
| composer_version | The composer version. | str | yes |

## Repository

The primary URL of this repo is [`https://git.coop/webarch/composer`](https://git.coop/webarch/composer) and this is where the [release notes](https://git.coop/webarch/composer/-/releases) are, it is also [mirrored to GitHub](https://github.com/webarch-coop/ansible-role-composer) and [available via Ansible Galaxy](https://galaxy.ansible.com/chriscroome/composer).

## Copyright

Copyright 2019-2024 Chris Croome, &lt;[chris@webarchitects.co.uk](mailto:chris@webarchitects.co.uk)&gt;.

This role is released under [the same terms as Ansible itself](https://github.com/ansible/ansible/blob/devel/COPYING), the [GNU GPLv3](LICENSE).
