Role Vector
=========

Role can install Vector.


Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------
Переменные для установки кредов default/main.yml:

|Переменная|Описание| 
|-|--------|
|vector_version|версия vector|

Dependencies
------------

Требуется роль clickhouse-role <br/>
[https://github.com/awertoss/clickhouse-role]

Example Playbook
----------------
```
hosts: vector
roles:
  - role: vector-role

```
License
-------

MIT

Author Information
------------------

Awertoss
