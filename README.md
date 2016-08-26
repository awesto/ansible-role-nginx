nginx
=====

This role installs nginx and installs vhost config files generated from
playbook-supplied templates.

Requirements
------------

None.

Role Variables
--------------

* `nginx_vhosts`: A list of mappings. Each item must have at least the keys
  `domainname` and `vhost_template`. You can add more keys to pass variables
  to your vhost template.


Dependencies
------------

None.

Example Playbook
----------------
```
- hosts: webservers
  roles:
  - nginx
  vars:
  - nginx_vhosts:
    - domainname: my.example.org
      vhost_template: nginx.conf.j2
```

License
-------

BSD

Author Information
------------------

René Fleschenberg <rene@fleschenberg.net>
