openstack-bmc
=============

Creates a vm image suitable for use in a baremetal Heat stack as described
in the corresponding Heat template.

Build the image using something like this::

    export ELEMENTS_PATH=~/tripleo-scripts/elements:/usr/share/tripleo-image-elements
    disk-image-create -o openstack-bmc fedora openstack-bmc vm

Note that the element is currently hard-coded for my devstack installation,
so you will likely need to change the OpenStack authentication details for
your environment.
