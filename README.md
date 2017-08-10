camkes-vm-manifest
==================
Initialize with: 
```
repo init -u https://github.com/GaloisInc/camkes-vm-manifest -m devel.xml -b devel
repo sync
```

If youa are using a config with `HUGEPAGES=y`, You will need to enable huge pages for QEMU/KVM, to do so edit `/etc/default/qemu-kvm` and set `KVM_HUGEPAGES=1` (see [here](https://help.ubuntu.com/community/KVM%20-%20Using%20Hugepages) for details)


The CAmkES VMM is a Virtual Machine Monitor that utilizes the CAmkES component platform.
Due to the static nature of CAmkES systems the VMM is specified at build time to run
on a particular hardware platform. Currently the VMM is mostly targeted to run on the
C162 platform from Aitech. There is also a configuration for running on generic x86
machines, but it has almost no hardware support.

For general instructions on how to use this repository, see [wiki.seL4.systems](https://wiki.sel4.systems/Getting%20started).

For general information about CAmkES see [the CAmkES pages on wiki.seL4.systems](https://wiki.sel4.systems/CAmkES).

For detailed information about CAmkES see documentation in [the camkes-tool repo](https://github.com/seL4/camkes-tool/blob/master/docs/index.md).

For detailed information about the VM on the C162 platform see the doucmention in [the camkes-vm repo](https://github.com/seL4/camkes-vm/blob/master/README.md).
