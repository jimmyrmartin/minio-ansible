Ansible playbook to install MinIO
=========

An easy to use and easy to maintain set of playbooks to make it easy to install MinIO in an air-gapped or online environment using best practices as found in the MinIO official docs. This is an official "unofficial" MinIO project. Your mileage may vary and official support is offered at best effort.


The playbook is intended to follow cloesly along with the documentation at:
https://min.io/docs/minio/linux/index.html to install a Multi-node Multi-disk (MNMD) installation.

The variables file in vars/main.yaml defines all of the variables that you need to define along with some examples directly from our documentation.

Requirements
------------

You will need to prepare your disks, disk labels, and make sure they are mounted before running the install playbook. We will be adding those steps as a task in the playbook soon. There is a node prep playbook you may use to help get that installed. It CAN be a destructive process so please be sure you know what you are doing.


Dependencies
------------

You will need to place the minio binary needed in files director. You can grab this from https://dl.min.io/server/minio/release/linux-amd64/minio


Example Usage
----------------
`ansible-playbook install-minio-playbook.yaml --inventory=minio-inventory --ask-become-pass`

# --ask-become-pass is the root password or your user password if needed.


License
-------

BSD

Author Information
------------------

Maintained by:

jimmrmartin - Jimmy Martin

mjkota - Mudit Jain
