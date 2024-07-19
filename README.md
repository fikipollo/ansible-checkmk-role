Role Name
=========

Install Checkmk in CentOS 7, Debian 10 or Ubuntu 20.04.
Checkmk is a software developed for IT Infrastructure monitoring. It is used for the monitoring of servers, applications, networks, cloud infrastructures (public, private, hybrid), containers, storage, databases and environment sensors.

Requirements
------------

None

Role Variables
--------------

By default this role will install Checkmk.
```

# The version for checkmk to install
checkmk_server_version: 1.6.0p30

# The name for the site to be created
checkmk_site_name: monitoring

# Password for the admin user
checkmk_cmkadmin_password: supersecret

```

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ansible-checkmk }

License
-------

MIT

Author Information
------------------

Rafa Hernandez (fikipollo)
