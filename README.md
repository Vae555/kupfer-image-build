# Xiaomi POCO F3 / Redmi K40 (alioth) Image

Prebuilt Arch Linux ARM image (kupfer) for the Xiaomi POCO F3 / Redmi K40 (alioth), featuring Plasma Mobile and automatic login support.

## Installation

Flash the image using fastboot:

```bash
fastboot erase dtbo_b
fastboot erase boot_b
fastboot flash userdata sm8250-xiaomi-alioth-barebone-full.img
fastboot flash boot_b sm8250-xiaomi-alioth-barebone-aboot.img
fastboot set_active b
fastboot reboot
```

For additional information about the Kupfer bootstrapping framework, see:

https://kupfer.gitlab.io/

## Default Credentials

Default user account:

| Username | Password |
| -------- | -------- |
| alarm    | alarm    |

It is strongly recommended to change the password after the first boot.

## User Interface

This image ships with **Plasma Mobile** as the default graphical environment.

## Automatic Login

Automatic login is configured through Plasma Login Manager (plasma-login-manager).

For configuration details, refer to the ArchWiki:

https://wiki.archlinux.org/title/Plasma_Login_Manager

## Kernel Updates

The kernel is updated continuously following the releases published in this repository.

To upgrade to the latest kernel version, install the kernel packages from the newest release.

## Notes

* Device: Xiaomi POCO F3 (alioth)
* Base system: Arch Linux ARM
* Desktop environment: Plasma Mobile
* Display manager: Plasma Login Manager
* Default account: `alarm`
* Automatic login enabled by default
