Intel OpenCL Install for Cluster in the Cloud
=============================================

This is an example playbook to demonstrate further customisation of the cluster.

Prerequisites
=============

This assumes you have already built a cluster with [Cluster in the Cloud
documentation](https://cluster-in-the-cloud.readthedocs.io/en/latest/)

It also assumes that the RPMs it needs have been copied in to
`/mnt/shared/apps/intel/opencl/`

To run the playbook
===================

```bash
[opc@mgmt ~]$ ls -l /mnt/shared/apps/intel/opencl/opencl-*.rpm > /dev/null || echo "You need to upload the RPMs"
[opc@mgmt ~]$ git clone https://github.com/ACRC/intel-opencl-playbook
[opc@mgmt ~]$ cd intel-opencl-playbook
[opc@mgmt intel-opencl-playbook]$ ansible-playbook -i /home/opc/hosts site.yml
```


