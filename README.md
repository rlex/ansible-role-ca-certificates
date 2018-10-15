#### ansible role for ca-certificates

Installs CAs (certificate authorities) to system and enables them.  
Supports RHEL and Debian-based systems.  
By default it will look for CAs in inventory_dir/files/ca-certificates and sync all of them with remote.  
[inventory_dir is pathname of the directory holding Ansible’s inventory host file](https://docs.ansible.com/ansible/2.4/playbooks_variables.html#magic-variables-and-how-to-access-information-about-other-hosts)

##### Params
There is not much to configure but you can override source directory:
```
ca_certificates_source: "{{inventory_dir}}/files/ca-certificates/*"
```
