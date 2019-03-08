Role Name
=========

Ansible role for deploying metricbeat on Mesos/Marathon, K8s or bare metal.

Role Variables
--------------

```yaml
metric_version:
elastic_host:
username:
password:
ssl_enabled:
ssl_verification:
index_name:
frequency:
```

Example Playbook
----------------

```yaml
    - hosts: servers
      roles:
         - indigo-dc.metricbeat
```

Author Information
------------------

Diego Ciangottini, INFN Perugia, 2019 - diego.ciangottini@pg.infn.it
