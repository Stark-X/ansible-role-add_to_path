add_to_path
=========

This is a ansible role to add a path to $PATH

Usage
-----

Copy the content below in the section [Example requirements.yml](#example-requirementsyml), and paste it as "requirements.yaml" to a playbook folder, execute `ansible-galaxy install -r requirement.yaml` to install this role

Requirements
------------

None

Role Variables
--------------

- `env_file_path`: the shell script to export "path" to $PATH
- `extra_path`: the "path" to export

Dependencies
------------

``` yaml
# mandatory
- src: https://github.com/Stark-X/ansible-role-mandatory.git
  version: 1.0
  name: manadtory
```

Example Playbook
----------------

``` yaml
- hosts: servers
  become: true
  tasks:
    - include_role:
        name: add_to_path
      vars:
        extra_path: /opt/foo/bin
```

Example requirements.yml
-----------------------

``` yaml
- src: https://github.com/Stark-X/ansible-role-add_to_path.git
  version: "1.0"
  name: add_to_path
```

License
-------

BSD

Author Information
------------------

Author: Stark-X

Mail: xiaojiezhi2@gmail.com

Blog: https://blog.stark-x.cn
