Ansible Role: New Bitrix host
=========

Configure host for Bitrix framework

Requirements
------------

None.

Role Variables
--------------
Available variables are listed below, along with default values (see `defaults/main.yml`):

Variable | Default | Description
---------|----------|---------
 `prjct_name` | example.com | Project name
 `db_name` | example | Database and user name
 `bitrix_passwd` | password | Password for user `bitrix`
 `db_passwd` | dbpass | Password for mysql user `$db_name`
 `mysql_root_pass` | test123 | Password for mysql `root` user

 
Dependencies
------------

None.

Example Playbook
----------------
```yml
    - hosts: new
      roles:
         - role: bitrix_host
           prjct_name: mysite
           db_name: mysite_crm
           bitrix_password: changeMe
           db_passwd: securePa$$w0rD
           mysql_root_pass: AnotherPass
```


License
-------

BSD

Author Information
------------------

This role was created in 2019 by [Vlad Bubnov](https://github.com/Faust13).
