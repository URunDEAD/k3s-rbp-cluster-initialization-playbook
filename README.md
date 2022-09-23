Raspberry Pi K3S Cluster Configurator
===

Just a tiny ansible playbook that boot starts my raspberry pi cluster.
OS: openSUSE jeOS for raspberry pi

It does the following:

- creates 2 backups of the system using timeshift before and after updating/upgrading.

- renames the machines: node0 (master), node1, node2...

- sets up ssh authentification via a key file that must be specified in inventory.yaml

- disables password authentification.

- install k3s on nodes & joins them
