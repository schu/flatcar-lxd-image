# flatcar-lxd-image

A helper script to import [Flatcar Linux](https://kinvolk.io/flatcar-container-linux/)
qemu virtual machine images into [LXD](https://linuxcontainers.org/lxd/).

## Usage

```
./flatcar-lxd-image [<channel> [<version> [<lxd name alias>]]]
```

Default `<channel>` and `<version>` is the latest stable release.

```
[...]

==> Added image 'flatcar-stable-2605.12.0'
==> Example launch command:

lxc launch flatcar-stable-2605.12.0 v1 --config security.secureboot=false

[...]

lxc image info flatcar-stable-2605.12.0

Fingerprint: 98ec788...
Size: 1035.88MB
Architecture: x86_64
Type: virtual-machine

[...]
```
