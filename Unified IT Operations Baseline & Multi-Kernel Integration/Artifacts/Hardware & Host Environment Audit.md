# Hardware & Host Environment Audit
This document is the technical baseline for the Unified IT Operations project. It gives a snapshot of the hardware and host OS setup used for virtualization. By auditing the host system resources like the CPU, RAM, and firmware, this artifact proves the environment is ready for WSL 2 and VirtualBox. It ensures all testing starts on a stable and fast foundation.

## Host System Specifications
- Device Model: HP Laptop 17-by4xxx
- Processor: 11th Gen Intel(R) Core(TM) i5-1135G7 @ 2.40GHz (4 Cores, 8 Logical Processors)
- Installed Physical Memory (RAM): 16.0 GB
- Host OS: Microsoft Windows 11 Home (Build 26200)
- BIOS Mode: UEFI (Secure Boot compatible)

## Virtualization Infrastructure
- Hypervisor Support: Intel VT-x (Verified via 11th Gen i5 Architecture)
- WSL 2 Backend: Enabled and integrated with Windows 11 Host
- VirtualBox Version: 7.0.x

## Baseline Resource Allocation
- Guest OS (Ubuntu): Allocated 4096 MB RAM
- Storage Allocation: 25.00 GB Dynamically Allocated VDI
- Graphics: VMSVGA with 3D Acceleration enabled
- Native Target Resolution: 1920 x 1080 (Full-Screen Mode)
