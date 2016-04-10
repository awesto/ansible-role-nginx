nginx
=====

This role is written for internal use by Awesto and not designed to cover
more general use-cases. You probably do not want to use it.

Requirements
------------

None.

Role Variables
--------------
```
nginx_vhosts:
  - domainname: my.example.org
    vhost_template: nginx.conf.j2
    listen_ip: 1.2.3.4
```

Dependencies
------------

None.

Example Playbook
----------------


License
-------

BSD

Author Information
------------------

René Fleschenberg <rene@fleschenberg.net>
