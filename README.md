Install Kubernetes
-----------------

Prerequisites
------------

1. Ubuntu 16.04 OS required
2. Master and Nodes should be reachable each other  or within the same subnet

Execution Procedure
-------------------

1. Update inventory/hosts file with IP and credetials
2. To install master node run the playbook,
   $ cd ansible
   $ ansible-playbook -i inventory/hosts playbook/kubernetes-master.yml
3. To install agent node,
   $ cd ansible
   $ ansible-playbook -i inventory/hosts playbook/kubernetes-node.yml

Installation will install docker as well
