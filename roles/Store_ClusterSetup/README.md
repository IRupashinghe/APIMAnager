# Ansible Role: ClusterSetup

This role is used for setting up server and cluster configurations for Enterprise Integrator . This role can be used in Ubuntu, RedHat7 and AmazonLinux

Requirments
--------------
Before you use this role you have to place you key file for inside file/* to ssh between nodes. That is used for Rsync purpose.

Role Variables
--------------

For this role there are few variables used:

You can define the cluster pattern either aws or wka for Well Known members.
```yaml
  membershipScheme: wka 
```

These Variables are only used when you select aws as your clustering pattern
```yaml
  access_key: 
  secret_key: 
  security_group: Ansible
  region: ap-south-1
```

You can change those variables as you like. According to you Database credentails. And also you can pick application domain as you like
```yaml
  domain: mitra.ei.com 
  doc_root: /opt//EI/wso2ei-6.1.1
  mysql_host: 172.31.27.53
  mysql_domain: carbondb.mysql-wso2.com
  app_user: mitra
```


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```yaml
    - hosts: servers
      roles:
         - ClusterSetup
```
License
-------

BSD

Author Information
------------------

This role was created in 2018 by [Iruka Avantha]
