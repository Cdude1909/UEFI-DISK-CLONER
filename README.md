# UEFI Disk Cloner

**OS-Free Data Acquisition Utility**

A standalone UEFI application for forensic disk cloning, designed to operate at the firmware level. This tool enables bit-perfect imaging of storage devices in air-gapped, locked, or tamper-sensitive environments without requiring any operating system credentials.

[![Platform](https://img.shields.io/badge/License-MIT-red)]()
[![Platform](https://img.shields.io/badge/Platform-UEFI-lightblue.svg)](https://uefi.org/)
[![Status](https://img.shields.io/badge/Status-BETA-yellow.svg)]()


---

### ⚠️ DISCLAIMER :
```
**IT DOES NOT DECRYPT THE ENCRYTPTED DISK [ BITLOCKER OR DISLOCKER or FILEVAULT ].
It will create replica of the disk in whichever state it was before the Shutdown.

** IT IS IN BETA STAGE , Please raise Queries if issues found which I am sure of.
```

## 🚀 Overview

The UEFI Disk Cloner is a forensic utility that executes as a `.efi` binary directly from the UEFI firmware. It bypasses the operating system entirely, providing unrestricted access to storage devices for digital forensics.

| Feature | Description |
| :--- | :--- |
| **No Password Required** | Bypasses OS-level authentication to access raw data. |
| **Bit-Perfect Sector Copy** | Creates exact, sector-by-sector clones of source disks, preserving all data including partition tables and unallocated space. |
| **Integrity Verification** | Supports SHA-256, SHA-1, and MD5 hashing for court-admissible evidence integrity. |
| **Pre-OS Execution** | Runs at the firmware level, ensuring zero interference from the target operating system. |

---

## ✨ Key Features

- **UEFI Native Application**: Runs as a standalone `.efi` binary, bootable from a USB drive.
- **Crash-Resumable Cloning** : Saves progress to NVRAM, resuming multi-hour imaging operations after a power failure without restarting.
- **Firmware-Safe I/O Scheduling**: Prevents hardware timeouts, ensuring reliable operation on slow or failing drives.
- **Cross-Platform Compatibility**: Works on any x86_64 system with UEFI firmware, including Intel MacBooks.
- **Real-World Validation**: Successfully deployed in over 21 real forensic investigations.

---

## 🛠️ Basic Architecture
<img width="648" height="592" alt="x" src="https://github.com/user-attachments/assets/9e4fed7d-cc3e-4985-9ee5-7c09b8f8e164" />

