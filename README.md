Role Vector
=========

Role can install Vector.


Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

|Переменная|Описание| 
|-|--------|
|vector_version|версия vector|

Dependencies
------------

Требуется роль clickhouse-role <br/>
[https://github.com/awertoss/clickhouse-role]

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

MIT

Author Information
------------------

Awertoss
