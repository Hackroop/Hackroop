# Making SanDisk Extreme 55AE Media Bootable

## Disclaimer

This guide is provided for informational and educational purposes only. Proceed at your own risk. Always back up important data before performing such tasks. The author or publisher of this guide is not responsible for any data loss, hardware damage, or other potential issues that may arise.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Making a Bootable Linux SSD (Kali Linux)](#making-a-bootable-linux-ssd)
  - [Mac/Linux](#maclinux)
  - [Windows](#windows)
- [Making a Bootable Windows SSD](#making-a-bootable-windows-ssd)
  - [Mac](#mac)
  - [Windows](#windows-1)
- [Note](#note)
- [Caution](#caution)

---

## Prerequisites

- **Download ISO Files**: Download the Kali Linux ISO from [Kali Linux Download Page](https://www.kali.org/get-kali/). For Windows, get the ISO from [Microsoft's Website](https://www.microsoft.com/en-us/software-download/windows10).

- **BalenaEtcher**: Download BalenaEtcher from [here](https://www.balena.io/etcher/) for writing the Linux ISO to the SSD.

- **UNetbootin**: Download UNetbootin from [here](https://unetbootin.github.io/) for creating a bootable Windows SSD on Mac.

---

## Making a Bootable Linux SSD (Kali Linux)

### Mac/Linux

1. **Connect the SSD**: Plug in your SanDisk Extreme 55AE Media.

2. **Open BalenaEtcher**: 
  - Run BalenaEtcher and click `Flash from file`.
  - Browse to the Kali Linux ISO and select it.

3. **Select Target Drive**:
  - Click on `Select target`.
  - Choose your SanDisk Extreme 55AE Media SSD.

> **Caution**: Make sure you've selected the correct drive.

4. **Click Flash**:
  - Click `Flash!`.

### Windows

1. **Download Rufus**: Download Rufus from [here](https://rufus.ie/).

2. **Open Rufus and Configure**:
  - Run Rufus, select the Kali Linux ISO, and choose your SanDisk Extreme SSD.

3. **Start the Process**: 
  - Click `Start`.

> **Caution**: This will erase all data on the target drive.

---

## Making a Bootable Windows SSD

### Mac

1. **Download UNetbootin**: Download and open UNetbootin.

2. **Configure UNetbootin**:
  - Select `Disk Image` and point to your Windows ISO.
  - Select your SanDisk Extreme 55AE Media SSD as the target.

> **Caution**: Make sure you've selected the correct drive.

3. **Start the Process**:
  - Click `OK`.

### Windows

1. **Use Rufus**: Follow the same steps as for Kali Linux but use the Windows ISO this time.

> **Caution**: This will erase all data on the target drive.

---

## Note

- Writing an ISO to an SSD will make the entire SSD bootable, not just a partition.
- Booting from an external SSD depends on BIOS or UEFI settings.

## Caution

- Proceed cautiously.
- Back up important data before starting.

