graphite
========

Graphite installed from RPMs and using Apache proxy and SQLite DB.


Example
-------

```
---

# Example of how to use the role
- hosts: myhost
  roles:
    - graphite
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


License
-------

MIT


Author
------

Jiri Tyr
