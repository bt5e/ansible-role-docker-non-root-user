# ansible-role-docker-non-root-user
Ansible Role - Manage docker as a non root user

Docker non-root user setup based on: https://docs.docker.com/engine/installation/linux/linux-postinstall/#manage-docker-as-a-non-root-user

## Usage
requires `non_root_docker_users` variable listing users to be able to manage docker

    - { role: docker-non-root-user, non_root_docker_users: vagrant }