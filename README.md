# KSM init script

[Kernel Samepage Merging (KSM)](https://www.kernel.org/doc/Documentation/vm/ksm.txt) is a Kernel-powered memory-saving de-duplication
daemon that periodically scans the whole memory, looking for pages that can be
merged together in order to save memory.

This init script is used to enable KSM on boot time and see how much memory it's
saving in a human-friendly way.



## Dependencies

* [OpenRC](https://github.com/OpenRC/openrc) (duh)
* [CONFIG_KSM](https://www.kernel.org/doc/Documentation/vm/ksm.txt)=y
* [CONFIG_SYSFS](https://www.kernel.org/doc/Documentation/filesystems/sysfs.txt)=y
* [numfmt (coreutils)](https://www.gnu.org/software/coreutils/manual/html_node/numfmt-invocation.html)
* getconf (glibc)
