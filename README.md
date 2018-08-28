ansible-role-pg-stat-statements
===============================

[![Build Status](https://travis-ci.org/kevincoakley/ansible-role-pg-stat-statements.svg?branch=master)](https://travis-ci.org/kevincoakley/ansible-role-pg-stat-statements)

Installs the pg_stat_statements for PostgreSQL 10 - https://www.postgresql.org/docs/current/static/pgstatstatements.html . Tested with pg_stat_statements 1.5 on CentOS 7.

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml and the example inventory below

Dependencies
------------

None

Example Playbook
----------------

    - name: Test the pg_stat_statements role for CentOS
      hosts: stat-statements
      become: yes
      become_method: sudo
    
      roles:
        - ansible-role-pg-stat-statements
    
      tags:
        - stat-statements

License
-------

BSD

Author Information
------------------

Kevin Coakley (https://github.com/kevincoakley)