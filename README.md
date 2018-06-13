# KSM init script

Kernel Samepage Merging (KSM) is a Kernel-powered memory-saving de-duplication
daemon that periodically scans the whole memory, looking for pages that can be
merged together in order to save memory.

This init script is used to enable KSM on boot time and see how much memory it's
saving in a human-friendly way.

https://www.kernel.org/doc/Documentation/vm/ksm.txt

## Dependencies

* OpenRC (duh)
* CONFIG_KSM
* CONFIG_SYSFS
* numfmt (coreutils)
* getconf (glibc)
