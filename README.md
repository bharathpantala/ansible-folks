# This repo is used to hold the deployment automation using Ansible.

*We will be adding the documentation of how to use this.*


## Install Ansible on Debian. 
* To install Ansible  run the below command
```bash
sudo apt-get update
sudo apt-get install -y ansible
```
## Install Ansible on Redhat/CentOS
* To install Ansible  run the below command
```bash
sudo yum update -y
sudo yum install -y ansible
```


* Write an `ansible.cfg` file and place it in a location where ansible can pick it up, either in `/etc/ansible/ansible.cfg` or in `$HOME/.ansible.cfg`. It should have the below contents.
```
[defaults]
lookup_plugins = /home/<user-name>/.ansible/roles/azure.azure_preview_modules/lookup_plugins
```

## Installing `pip` on RHEL
* Incase `pip` command is not available, please follow this guide to get `pip` working on RHEL:
    * [How to install pip on Red Hat Enterprise Linux?](https://access.redhat.com/solutions/1519803)
