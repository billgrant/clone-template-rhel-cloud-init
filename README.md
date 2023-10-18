# clone-template-rhel-cloud-init

This repo contains a working terraform example that creates a CentOS 8 VM from a template, configures the VM with cloud-init.

It also uses the Terraform built in function [templatefile](https://developer.hashicorp.com/terraform/language/functions/templatefile) to render variables into the cloud-init files.

 **Note: cloud-init must be installed on your template.**

To comfirm run the following

```
rpm -qa | egrep cloud-init
```

Example output
```
cloud-init-23.1.1-11.el8.noarch
```

If the command returns nothing, then you will have to install cloud-init

```
sudo yum install cloud-init
```