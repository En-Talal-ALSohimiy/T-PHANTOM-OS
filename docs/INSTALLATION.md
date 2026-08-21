# T‑PHANTOM OS Installation Guide

This guide covers installing T‑PHANTOM OS as the primary operating system on a dedicated machine.

> **Warning:** selecting the entire disk during installation can erase all existing partitions, files, and operating systems on that disk.

## Before you begin

- Back up all important data.
- Verify the SHA‑256 of `T-PHANTOM.iso` against `SHA256SUMS`.
- Use a USB drive large enough for the ISO.
- Prefer UEFI boot mode on modern hardware.
- If Secure Boot blocks startup, disable it temporarily in firmware settings unless/until a signed boot chain is provided for the release.

## Create the USB installer

On Linux, identify the USB device first:

```bash
lsblk -o NAME,SIZE,MODEL,TRAN,MOUNTPOINTS
```

Unmount any mounted USB partitions, replacing `/dev/sdX` with the actual USB device:

```bash
sudo umount /dev/sdX* 2>/dev/null || true
```

Write the ISO to the whole device, **not a partition**:

```bash
sudo dd if=T-PHANTOM.iso of=/dev/sdX bs=4M status=progress conv=fsync
sync
```

## Boot from USB

1. Restart the computer.
2. Open the firmware boot menu.
3. Select the USB entry, preferably the **UEFI** entry.
4. In the T‑PHANTOM boot menu, choose **Start installer**.

## Installer flow

The installer will guide you through:

1. Language selection.
2. Country/region.
3. Keyboard layout.
4. Network configuration.
5. Hostname configuration. The intended default hostname is `t-phantom`.
6. User and password setup.
7. Disk partitioning.
8. Base-system installation.
9. Bootloader installation.
10. Reboot into the installed system.

## Installing as the only operating system

For a dedicated T‑PHANTOM machine, choose the guided option that uses the entire target disk. Confirm the disk model and capacity before accepting destructive changes.

Do **not** continue if the selected disk contains data you need.

## First boot checks

After installation:

```bash
cat /etc/os-release
hostnamectl
findmnt /
systemctl --failed
```

Expected user-facing identity:

```text
T-PHANTOM OS
```

Expected hostname:

```text
t-phantom
```

If available, run the built-in system check:

```bash
tphantom-system-check
```

## Virtual machine testing

For QEMU/KVM, VirtIO graphics is recommended over legacy `std` VGA when possible:

```bash
qemu-system-x86_64 \
  -enable-kvm \
  -cpu host \
  -machine q35 \
  -m 4096 \
  -smp 4 \
  -device virtio-vga \
  -display gtk,grab-on-hover=off,show-cursor=on \
  -cdrom T-PHANTOM.iso \
  -boot d
```

## Release qualification note

A successful VM install does not prove universal hardware compatibility. Before broad deployment, validate at least UEFI boot, storage, graphics, Wi‑Fi, Ethernet, sound, suspend/resume, and shutdown/restart on representative physical hardware.
