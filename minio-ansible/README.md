Ansible playbook to install MinIO
=========

The playbook is intended to follow cloesly along with the documentation at:
https://min.io/docs/minio/linux/index.html to install a Multi-node Multi-disk (MNMD) installation.

The variables file in vars/main.yaml defines all of the variables that you need to define along with some examples directly from our documentation.

Requirements
------------

You will need to prepare your disks, disk labels, and make sure they are mounted before running the install playbook. We will be adding those steps as a task in the playbook soon. 


Dependencies
------------

You will need to place the minio binary needed in files director. You can grab this from https://dl.min.io/server/minio/release/linux-amd64/minio


License
-------

BSD

Author Information
------------------

Maintained by:
jimmrmartin - Jimmy Martin
mjkota - Mudit Jain
