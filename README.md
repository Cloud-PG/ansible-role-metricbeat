[![Build Status](https://travis-ci.org/Cloud-PG/ansible-role-metricbeat.svg?branch=master)](https://travis-ci.org/Cloud-PG/ansible-role-metricbeat)
Metricbeat ansible
=========

Ansible role for deploying metricbeat on Mesos/Marathon, K8s or bare metal.

Role Variables
--------------

```yaml
orchestrator:
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
---
- hosts: localhost
  remote_user: root
  roles:
    - cloud-pg.ansible_role_metricbeat
  vars:
    orchestrator: kubernetes or marathon
    metric_version: 6.2.4
    elastic_host: https://example.com:9204
    username: CHANGEME
    password: CHANGEME
    ssl_enabled: true
    ssl_verification: none
    index_name: metricbeat-k8s-6.2.4
    frequency: 30s
```

Author Information
------------------

Diego Ciangottini, INFN Perugia, 2019 - diego.ciangottini@pg.infn.it
