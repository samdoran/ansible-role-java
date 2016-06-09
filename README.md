Java
=========
[![Galaxy](https://img.shields.io/badge/galaxy-samdoran.java-blue.svg?style=flat)](https://galaxy.ansible.com/samdoran/java)
[![Build Status](https://travis-ci.org/samdoran/ansible-role-java.svg?branch=master)](https://travis-ci.org/samdoran/ansible-role-java)

Install Java.

Requirements
------------

None.

Role Variables
--------------

| Name              | Default Value       | Description          |
|-------------------|---------------------|----------------------|
| `java_packages` | `[]` | List of packages to install. Varies by distribution and version.  |

The versions avaialable vary by distribution and version. Here are the defaults:

| Distribution              | Distribution Version       | Java Package Name          |
|-------------------|---------------------|----------------------|
| Red Hat | all | java-1.8.0-openjdk |
| Ubuntu | 12.04, 14.04 | java-1.7.0-openjdk |
| Ubuntu | 16.04 | java-1.8.0-openjdk |

See `vars` for a list of available packages for each distribution.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: all
      roles:
         - samdoran.java

License
-------

MIT
