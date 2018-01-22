# Ansible Role: DbSetup

This role is used for configuring the Database related configurations for Enterprise Integrator . This role can be used in Ubuntu, RedHat7 and AmazonLinux


Role Variables
--------------

For this role there are few variables used

```yaml
    ---
  db_host: carbondb.mysql-wso2.com
  db_port: 3306
  db_user: regadmin
  db_password: regadmin
  doc_root: /opt/EI/wso2ei-6.1.1
  app_user: mitra
```
You can change those variables as you like. According to you Database credentails

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
    - hosts: servers
      roles:
         - DbSetup
```
License
-------

BSD

Author Information
------------------

This role was created in 2018 by [Iruka Avantha]
