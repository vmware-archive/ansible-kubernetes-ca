kubernetes-ca
=============

current version: 0.0.0
A role to create/use openssl to generate certificates for kubernetes nodes

Role Variables
--------------

Example Playbook
----------------

Example for bootstraping a SSL-protected etcd cluster with CoreOS

    - name: kubernetes ca
      hosts: ca
      roles:
        - role: "sigma.kubernetes-ca"
          kubernetes_master_group: "masters"

License
-------

MIT
