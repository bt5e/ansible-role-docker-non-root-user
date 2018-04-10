Ansible Role - Docker non-root User - CentOS
============================================

Ansible Role - Manage docker as a non root user

Docker non-root user setup based on: https://docs.docker.com/engine/installation/linux/linux-postinstall/#manage-docker-as-a-non-root-user

Requirements
------------

Assumes Docker is installed.

Role Variables
--------------

| Variable              | Required | Defaults | Comments  |
| --------------------- | -------- |--------- | --------- |
| non_root_docker_users | yes      |          | List of non-root users to be allowed to manage docker |

Dependencies
------------

- bt5e.docker-ce

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: bt5e.docker-non-root-user, non_root_docker_users: vagrant }

License
-------

MIT

Author Information
------------------

Ben Tse
