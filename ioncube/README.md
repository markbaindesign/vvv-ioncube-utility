# Ioncube VVV utility

Ioncube utility for VVV

This utility will set up [Ioncube](http://www.ioncube.com/) on your [VVV](https://github.com/Varying-Vagrant-Vagrants/VVV) installation.

## Usage

In your `vvv-custom.yml` file add under `utilities`:

```yml
utilities:
  core:
    - memcached-admin
    - opcache-status
    - phpmyadmin
    - webgrind
  ioncube:
    - ioncube
utility-sources:
  redis: https://github.com/dingo-d/redis-vvv-utility
```

The `core` utilities are there by default.

Once you add it, be sure you re-provision your VVV with `vagrant reload --provision`.
