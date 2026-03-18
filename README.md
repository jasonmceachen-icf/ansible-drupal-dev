# Installs a set of Drupal development tools on your Mac

UNTESTED!!!

This was built behind me as I installed development tools on my macbook.

## Note



## Installation

Running the script in bin/bootstrap will install homebrew, use homebrew to install pipx, and use pipx to install Ansbile.
Once that is complete, it runs a playbook which additionally installs Lando and VSCode with Drupal related extensions.

Start the installer:
```bash
bin/bootstrap
```

and verify with 
```bash
ansible all --list-hosts
```

which should return one host at localhost
```bash
  hosts (1):
    localhost
```


## Updates

You can run the playbooks individually or in the collected devEnvironment to update all packages and 
extensions.


## Bibliography

[Configuring Visual Studio Code](https://www.drupal.org/docs/develop/development-tools/editors-and-ides/configuring-visual-studio-code)

[Get Lando](https://lando.dev/download)

[How to Use Ansible to Manage Homebrew Packages on macOS]( https://oneuptime.com/blog/post/2026-02-21-ansible-manage-homebrew-packages-macos/view)
