# srsLTE ansible-playbook
Mihai Idu - 2019

## Description 

This is a ansible-playbook to automate the deployment, installation and configuration of the srsLTE.

## Execution Instructions

Before lunching the below command, please check the following set of files that respect the configuration that you want:

-   /roles/files/srsenb/*                   - those files should include the eNB configurations

-   /roles/files/srsepc/*                   - those files should includethe EPC configurations

-   inventory-srsLTE                        - this file should include the hostname of all the 
physical or virtual machines and IPs where do you want to install the srsLTE

```
$ ansible-playbook -i inventory-srsLTE -u <USERNAME> -bkK playbook.yml
```

After lunching the above command the ssh password for the choosen <USERNAME> it will be requested by the ansible-playbook in order to create the ssh connection to the desired host.

# Support
Mailing to the followin address: idumihai16@gmail.com
