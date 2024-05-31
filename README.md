# minio-ansible
Ansible Playbook to install MinIO in a more easily maintained way

Currently, there is an Ansible role that has been created and forked, however, it lacks a lot of features you may want, as well as not being easily maintained by someone who may not be familiar with Ansible.

The aim here is to create an easier maintained and used set of playbooks as well as to create a "node prep" playbook.

Design goals:

- The playbook should be able to support airgapped and "online" installs.
- Easily updated by someone new to Ansible
- Self-documenting
- Node prep and MinIO install seperated by concerns
