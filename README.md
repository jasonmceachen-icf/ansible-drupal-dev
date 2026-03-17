# Installs a set of Drupal development tools on your Mac

UNTESTED!!!

This was built behind me as I installed development tools on my macbook.

## Note



## Installation

Running the script in bin/bootstrap will install homebrew, use homebrew to install pipx, and use pipx to install Ansbile.
Once that is complete, it runs a playbook which additionally installs Lando and VSCode with Drupal related extensions.

Start the installer:
```
bin/bootstrap
```

and verify with 
```
ansible all --list-hosts
```
which should return one host at localhost
```
  hosts (1):
    localhost
```


## Updates

You can run the playbooks individually or in the collected devEnvironment to update all packages and 
extensions.
