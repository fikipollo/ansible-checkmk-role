Role Name
=========

Install Checkmk in CentOS 7.
Checkmk is a software developed for IT Infrastructure monitoring. It is used for the monitoring of servers, applications, networks, cloud infrastructures (public, private, hybrid), containers, storage, databases and environment sensors.

Requirements
------------

None

Role Variables
--------------

By default this role will install Checkmk.
```

# The version for checkmk to install
checkmk_server_version: 1.5.0p11

# The name for the OS (el7 is CentOS 7)
checkmk_server_dist: el7

# The name for the site to be created
checkmk_site_name: monitoring

# Password for the admin user
checkmk_cmkadmin_password: supersecret

# The URL for the official checkmk repository
checkmk_repo_url: https://checkmk.de/support/{{ checkmk_server_version }}/check-mk-raw-{{ checkmk_server_version }}-{{ checkmk_server_dist }}-38.x86_64.rpm

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
