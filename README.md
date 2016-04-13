vicenteg.filebeat
=========

Install filebeat, and configure to send logs to logstash.

Requirements
------------


Role Variables
--------------

```
logstash_hosts: '["1.2.3.4:5044", "1.2.3.5:5044"]'
```

Dependencies
------------

Example Playbook
----------------

```
- hosts: cluster
  roles:
    - { role: ansible-filebeat, logstash_hosts: '["1.2.3.4:5044", "1.2.3.5:5044"]' }
  environment:
    proxy_env:
      http_proxy: http://172.16.1.58:3128
      https_proxy: http://172.16.1.58:3128
```

License
-------

Apache

Author Information
------------------

Vince Gonzalez
