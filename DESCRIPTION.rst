|app|
=====

Deploy and configure docker daemon,

Requirements
------------

ansible-role-smd-bootstrap

Dependencies
------------

N/A

Example Playbook
----------------

.. code::

  - hosts: servers
    roles:
      - { role: ansible-role-smd-docker }

