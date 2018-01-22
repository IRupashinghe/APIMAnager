# Ansible Role: EISetup

This role is used for Downloading the Fresh Enterprise Integrator to the Server. This role can be used in Ubuntu, RedHat7 and AmazonLinux


Role Variables
--------------

For this role there is one variable used for definig the App User.

```yaml
    app_user: mitra
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
    - hosts: servers
      roles:
         - EISetup
```
License
-------

BSD

Author Information
------------------

This role was created in 2018 by [Iruka Avantha]
