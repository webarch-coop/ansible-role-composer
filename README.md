# Install Composer

This role installs Composer from
[GitHub](https://github.com/composer/composer/releases).

If `composer_version` is left to the default of `latest` then the latest
version will be installed, if it is specified using a version tag, for example:

```yml
composer_version: 2.0.11
```

Then the specified version will be installed.
