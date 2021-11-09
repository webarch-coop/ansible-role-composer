# Ansible Composer Role

This Ansible role downloads Composer from
[GitHub](https://github.com/composer/composer/releases), checks the GPG
signature and then installs it to `/usr/local/bin/composer`.

If `composer_version` is left to the [default](defaults/main.yml) of `latest`
then the latest version will be installed, if it is specified using a version
tag, for example:

```yml
composer_version: 2.1.12
```

Then the specified version will be installed.

The [localhost](https://git.coop/webarch/localhost) repo can be used to run
this role on the `localhost`.
