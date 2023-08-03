*VMware has ended active development of this project, this repository will no longer be updated.*

kubernetes-ca
=============

current version: 0.0.1
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

If deploying master nodes in HA configuration, following variables can be specified:
          kubernetes_master_elb_ip: <MASTER_LOADBALANCER_IP>
          kubernetes_master_elb_dns_name: <MASTER_LOADBALANCER_DNS_NAME>
          kubernetes_master_elb_cname: <MASTER_LOADBALANCER_CNAME>

License
-------

Copyright 2015 VMware, Inc.  All rights reserved.

SPDX-License-Identifier: MIT OR GPL-3.0-only

This code is Dual Licensed MIT or GPLv3
