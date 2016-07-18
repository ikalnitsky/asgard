Asgard
======

Asgard is a baremetal management and provisioning setup that's based on
standalone Ironic with nodes auto-discovery. The main idea is to move
as much business logic as possible from RAM disk (boot image) to server
side. That basically means the following things:

* Simple agent inside PXE boot image without inspection.
* Inspection made by [Ironic Ansible Driver].
* Deployment made by [Ironic Ansible Driver].
* No-auth endpoint for auto-discovery.

On the first glance it may be very similar to [Bifrost], another solution
for standalone Ironic, however unlike the last one Asgard is focusing
on auto-discovery and Ansible-based driver. Though no one say it
won't be integrated to [Bifrost] one day. :)


[Bifrost]: https://github.com/openstack/bifrost
[Ironic Ansible Driver]: https://review.openstack.org/#/c/325974/7
