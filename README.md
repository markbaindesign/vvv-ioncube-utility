# Ioncube VVV utility

Ioncube utility for VVV

This utility will set up [Ioncube](http://www.ioncube.com/) on your [VVV](https://github.com/Varying-Vagrant-Vagrants/VVV) installation. This is required by the [Memberium](https://memberium.com/) WordPress plugin.

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
  ioncube: https://github.com/markbain/vvv-ioncube-utility
```

The `core` utilities are there by default.

Once you add it, be sure you re-provision your VVV with `vagrant reload --provision`.
