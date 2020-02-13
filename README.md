add_to_path
=========

This is a ansible role to add a path to $PATH

Requirements
------------

None

Role Variables
--------------

env_file_path: the shell script to export "path" to $PATH
extra_path: the "path" to export

Dependencies
------------

Stark-X.mandatory
src: https://github.com/Stark-X/mandatory
version: master

Example Playbook
----------------

``` yaml
- hosts: servers
  tasks:
    - include_role:
     name: Stark-X.add_to_path
    vars:
      extra_path: /opt/foo/bin
```

License
-------

BSD

Author Information
------------------

Author: Stark-X
Mail: xiaojiezhi2@gmail.com
Blog: https://blog.stark-x.cn
