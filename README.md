# Installs a set of Drupal development tools on your Mac

## NOTE

LIGHTLY TESTED!!!

This was built behind me as I installed development tools on my macbook.

## What it does

Running the script in bin/bootstrap will install homebrew, use homebrew to install pipx, and use pipx to install Ansbile.
Once that is complete, it runs a playbook which additionally installs

- Lando
- VSCode with Drupal related extensions
- git ssh commit signing

## Installation

_Note_ You will need to enter your password for the first run so you can become a passwordless sudo user

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

## After installation

Ansible can only do so much, here's where you the user come in!

- [ ] Add your signing key to github

- [ ] Get the updated prompt by running `source ~/.zshrc`

## Updates

You can run the playbooks individually or in the collected dev-environment playbook to update all packages and extensions.

## Bibliography

[Configuring Visual Studio Code](https://www.drupal.org/docs/develop/development-tools/editors-and-ides/configuring-visual-studio-code)

[Get Lando](https://lando.dev/download)

[How to Use Ansible to Manage Homebrew Packages on macOS](https://oneuptime.com/blog/post/2026-02-21-ansible-manage-homebrew-packages-macos/view)

[Installing or updating to the latest version of the AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

[signing commits](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits)

[customizing my zsh prompt](https://dev.to/cassidoo/customizing-my-zsh-prompt-3417)
