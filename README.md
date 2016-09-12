# Ansible Playbook: Install Jetbrains applications
This playbook allows you to install a single or a set of the Jetbrains application on linux or OSX

## Installing a single app
You can install a single application super easy by just kicking off the specific playbook

``` bash
# Installing pycharm
ansible-playbook install_pycharm.yml
```

## Installing multiple apps

``` bash
# Install all apps
ansible-playbook install_jetbrains_products.yml

# Install a subset of apps (EX: pycharm, rubymine and web storm)
ansible-playbook install_jetbrains_products.yml --tags="pycharm,rubymine,webstorm"
```