Ansible Role: OpenStack Neutron Controller
==========================================

This role installs and configures OpenStack Neutron Controller Node on EL7 system.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`)

    host: controller

Host that runs Neutron services.

    nova_host: controller
    nova_password:

Nova credentials.

    keystone_host: controller
    keystone_password:

Keystone credentials.

    keystone_admin_password:

Password for admin Keystone user.

    mysql_host: controller
    mysql_password:

MySQL credentials.

    rabbitmq_host: controller
    rabbitmq_user:
    rabbitmq_password:

RabbitMQ credentials.

    metadata_secret:

Secret token for metadata proxy.

    region: RegionOne

OpenStack region.

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - binarycode.openstack-neutron-controller

License
-------

BSD

Author Information
------------------

[Igor Sidorov](https://github.com/binarycode)
