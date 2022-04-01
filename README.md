# Webarchitects Ansible Composer Role

[![pipeline status](https://git.coop/webarch/composer/badges/master/pipeline.svg)](https://git.coop/webarch/composer/-/commits/master)

An Ansible role which downloads Composer from [GitHub](https://github.com/composer/composer/releases), checks the GPG signature and then installs it to `/usr/local/bin/composer`, there are two [default variables](defaults/main.yml):

| Variable name        | Default value    | Comment                                              |
|----------------------|------------------|------------------------------------------------------|
| `composer_php`       | `php`            | The PHP executable, a full path can be specified     |
| `composer_version`   | `latest`         | The version, can be set to a specific version number |

If the `composer_php` version is `< 7.2.5` then the 2.2 LTS version of Composer is installed when `composer_version` is set to `latest`, if the version of PHP is `>= 7.2.5` then the latest stable version is installed, see the [release announcement for Composer `2.3.0`](https://blog.packagist.com/composer-2-3/) and the *Manual Download* section of the [Composer download page](https://getcomposer.org/download/).

The primary URL of this repo is [`https://git.coop/webarch/composer`](https://git.coop/webarch/composer) however it is also [mirrored to GitHub](https://github.com/webarch-coop/ansible-role-composer) and [available via Ansible Galaxy](https://galaxy.ansible.com/chriscroome/composer).

The [localhost](https://git.coop/webarch/localhost) repo can be used to run this role on the `localhost`.
