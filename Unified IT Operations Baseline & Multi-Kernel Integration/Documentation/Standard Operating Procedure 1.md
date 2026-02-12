# Standard Operating Procedure (SOP)

## 1. Baseline Establishment (Host Recovery)
- Execute full storage sanitation and a clean-slate Windows 11 Home deployment via the Media Creation Tool to eliminate legacy driver interference.
- Enable hardware-level virtualization (Intel VT-x) within the BIOS/UEFI firmware.

## 2. Native Kernel Integration (WSL 2)
- Initialize the Virtual Machine Platform and WSL backend via Windows Terminal.
- Deploy Ubuntu 24.04 LTS and verify shell accessibility through UNIX credential configuration.

## 3. Virtualized Kernel & Hardening (VirtualBox)
- Configure a Type-2 Hypervisor instance with 25GB of allocated storage for Ubuntu 24.04.3 LTS.
- CLI Recovery Pivot: In the event of a graphical installer hang during the Ubuntu Pro setup, pivot to the terminal to manually finalize registration and system attachment.
- Finalize security hardening by attaching a personal Ubuntu Pro token and executing a verified 105.4 MB system update cycle.

## 4. Workspace Optimization
- Install VirtualBox Guest Additions to enable bidirectional clipboard support.
- Manually map the display resolution to 1600x900 to resolve scaling and "letterboxing" issues.

#

*Updated as needed. Last update: February 12, 2026*
