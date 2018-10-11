Welcome to ansible-role-smd-docker Ansible Role
===============================================

ansible-role-smd-docker
-----------------------

Deploy and configure docker daemon,

### Requirements

ansible-role-smd-bootstrap

### Dependencies

N/A

### Example Playbook

    - hosts: servers
      roles:
        - { role: ansible-role-smd-docker }

Default variables
-----------------

#### Sections

-   Configuration

### Configuration

`smd_docker_storage_device`

> Drive where docker thin LVM will be created

    smd_docker_storage_device: /dev/vdb

`smd_docker_vg_size`

> Size on the thin volume

    smd_docker_vg_size: 100%

`smd_docker_bind_network`

> Network where docker daemon will listen

    smd_docker_bind_network: DEFAULT

`smd_docker_bind_port`

> Port where docker daemon will listen

    smd_docker_bind_port: 2376

`smd_docker_proxy`

> Proxy to connect to artifactory

    smd_docker_proxy: http://prod-epg-ost-proxy-01.hi.inet:6666

`smd_docker_options`

> Docker daemon options

    smd_docker_options:
      bip: 192.168.200.1/24
      userland_proxy: false
      registries:
        - artifactory.hi.inet

`smd_docker_packages`

> Docker packages to install

    smd_docker_packages:
      - docker-1.10.3-46.el7.10.x86_64
      - docker-selinux-1.10.3-46.el7.10.x86_64
      - python-docker-py-1.7.2-1.el7.noarch

Changelog
---------

This project adheres to Semantic Versioning and human-readable
changelog.

### ansible-role-smd-docker master - 2017/09/18

##### Added

-   First addition

##### Changed

-   First change

### ansible-role-smd-docker v0.0.1 - 2017/09/18

##### Added

-   Initial version

Copyright
---------

ansible-role-smd-docker Ansible Role

Copyright (c) 2017, Fernando Gonzalez
\<<fernando.gonzalezlara.ext@telefonica.com>\>

Telefonica I+D
