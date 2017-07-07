# HSBXL Dashboard 'Vagrant + Ansible' dev box


Development vagrant setup. 
Starts a new box in your virtualbox and initiates a complete development environment within this VM machine.

## VM ingredients
Debian 9, Drupal 8, adminer, drupal-console, drush, mailhog, memcached, pimpmylog, solr, varnish, xdebug




## Quickstart

You will need the following installed on your machine:
- virtualbox https://www.virtualbox.org/wiki/Downloads
- vagrant https://www.vagrantup.com/docs/installation
- vagrant hostsupdater plugin https://github.com/cogitatio/vagrant-hostsupdater#installation
- composer https://getcomposer.org/doc/00-intro.md

```
$ git clone https://github.com/hsbxl/dashboard.git
$ cd dashboard
$ composer install
$ DRUPALVM_ANSIBLE_ARGS='--ask-vault-pass' vagrant up
```

you will be asked for a vault password at one moment. 
This is a passphrase to decrypt our secrets.yml file, which contains some needed vars.

The HSBXL dashboard will be available at http://local.dashboard.hsbxl.be

https://github.com/hsbxl/dashboard