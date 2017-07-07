# HSBXL Dashboard 'Vagrant + Ansible' dev box

https://github.com/hsbxl/dashboard

## Quickstart
```
$ git clone https://github.com/hsbxl/dashboard.git
$ cd dashboard
$ composer install
$ DRUPALVM_ANSIBLE_ARGS='--ask-vault-pass' vagrant up
```

you will be asked for a vault password at one moment. 
This is a passphrase to decrypt our secrets.yml file, which contains some needed vars.