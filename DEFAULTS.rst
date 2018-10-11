.. vim: foldmarker=[[[,]]]:foldmethod=marker

Default variables
=================

.. contents:: Sections
   :local:

Configuration
-------------
.. envvar:: smd_docker_storage_device

   Drive where docker thin LVM will be created

::

  smd_docker_storage_device: /dev/vdb



.. envvar:: smd_docker_vg_size

   Size on the thin volume

::

  smd_docker_vg_size: 100%



.. envvar:: smd_docker_bind_network

   Network where docker daemon will listen

::

  smd_docker_bind_network: DEFAULT



.. envvar:: smd_docker_bind_port

   Port where docker daemon will listen

::

  smd_docker_bind_port: 2376



.. envvar:: smd_docker_proxy

   Proxy to connect to artifactory

::

  smd_docker_proxy: http://prod-epg-ost-proxy-01.hi.inet:6666



.. envvar:: smd_docker_options

   Docker daemon options

::

  smd_docker_options:
    bip: 192.168.200.1/24
    userland_proxy: false
    registries:
      - artifactory.hi.inet



.. envvar:: smd_docker_packages

   Docker packages to install

::

  smd_docker_packages:
    - docker-1.10.3-46.el7.10.x86_64
    - docker-selinux-1.10.3-46.el7.10.x86_64
    - python-docker-py-1.7.2-1.el7.noarch





