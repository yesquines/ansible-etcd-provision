ETCD PROVISION
=========

Requirements
------------

-

Role Variables
--------------

* KVDB Vars:
  - `etcd_version`
  - `etcd_data_dir`
  - `etcd_cluster_token`
  - `etcd_secure`

See [defaults/main.yml](./defaults/main.yml)

Dependencies
------------

* Remote access 
* Inventory
  - Refering to the group as `etcd_machines`

Example Playbook
----------------

See 
* [playbook-etcd.yaml](./playbook-etcd.yaml) - For provisioning without certificates
* [playbook-etcd-auth.yaml](./playbook-etcd-auth.yaml) - For provisioning with certificates

Execution example:

* `ansible-playbook -i inventory playbook.yaml` 

