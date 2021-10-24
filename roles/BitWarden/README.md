# Issues
Ansible expect does not seem to properly handle the bitwarden install script, so sadly that part needs to be done by hand. This also mean until I figure this out the following vars are unused:  
``` yaml
bitwarden_use_ssl: false
bitwarden_generate_ssl: false
bitwarden_database_name: vault
bitwarden_instalation_id:
bitwarden_instalation_key:
```
