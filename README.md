graphite
========

Graphite installed from RPMs and using Apache proxy and SQLite DB.


Example
-------

```
---

# Example of how to use the role
- hosts: myhost1
  roles:
    - graphite

# Example of how to set additional params
- hosts: myhost2
  roles:
    - role: graphite
      graphite_timezone: US/Central
      graphite_apache_cors: yes
```


Role variables
--------------

List of variables used by the role:

```
# Default timezone of the graphite data
graphite_timezone: America/Chicago

# Default secret key used by Graphite
graphite_secret_key: TopSecretKey

# Default Apache port number for Graphite vhost
graphite_apache_port: 8080

# CORS (Cross Origin Resource Sharing) - required if Grafana is hosted on
# different domain than Graphite
graphite_apache_cors: false

# Default CORS origin
graphite_apache_cors_origin: '*'
```

Dependencies
------------

* [`carbon`](https://github.com/picotrading/ansible-carbon) role


License
-------

MIT


Author
------

Jiri Tyr
