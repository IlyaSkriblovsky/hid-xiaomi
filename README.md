# hid-xiaomi
HID driver for Linux that supports side buttons of Xiaomi Mi Silent Mouse

## UPDATE

This kernel module was included in upcoming 5.16 kernel release. This package only makes sense now for kernel ≤5.15.

## Installation instruction (Ubuntu & other Debian-based distros):

First download .deb package from [Releases](https://github.com/IlyaSkriblovsky/hid-xiaomi/releases).

### Install the package:
`sudo dpkg -i hid_xiaomi-dkms_1.0_amd64.deb`

### Insert the kernel module
`sudo modprobe hid_xiaomi`

Side buttons on your mouse should start to work immediately. But you will need to do `modprobe hid_xiaomi` after each reboot.

To automatically insert the module while booting add `hid_xiaomi` to your `/etc/modules` file.
