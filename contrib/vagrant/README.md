Vagrant for Asgard
==================

Vagrant for Asgard is a regular Vagrant script that bootstraps 2 VMs as
proof-of-concept. It's a good (and recommended) way to play around with
standalone Ironic as well as Asgard itself.

As it as mentioned above, there are 2 VMs and here they are:

1. **master**

   Master node is where all needed software is installed, including but
   not limited to standalone Ironic, PXE server and so on. It's usually
   a point of interaction with end users.

2. **slave**

   Slave, on the other hand, is a baremetal analog that must be booted
   and discovered by master's management software.


Usage
-----

In order to bootstrap them one should use a usual Vagrant command:

    $ vagrant up
