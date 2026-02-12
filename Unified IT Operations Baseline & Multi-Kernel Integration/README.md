# Unified IT Operations Baseline & Multi-Kernel Integration
By Quinisha Cockheran

## Executive Summary
This project details the systematic re-engineering of a primary workstation to serve as a high-performance laboratory for multi-OS experimentation. Following a critical failure of secondary kernel integration (WSL 2), a strategic decision was made to execute a full system recovery to ensure a "Pristine State" baseline optimized for virtualization and cross-platform development.

## Purpose
The objective was to establish a dedicated IT Operations environment on a clean hardware-software baseline. This ensures 100% compatibility for parallel Linux environments, allowing for simultaneous native kernel operations (WSL 2) and full-system virtualization (VirtualBox) without legacy system interference.

## Tools Used
Windows 11 Pro: Host Operating System and primary administrative environment.
Windows Media Creation Tool: Used for host OS deployment and full storage sanitation.
Windows Terminal: Primary interface used to initialize the WSL 2 backend and manage Linux distributions.
Oracle VM VirtualBox 7.0: Type-2 Hypervisor used for full-system GUI Linux testing.
BIOS/UEFI Firmware: Configured for hardware-level virtualization support (Intel VT-x).
GitHub: For repository management, version control, and Technical SOP documentation.

## Methodology
Phase 1: Host Recovery & Hardware Optimization
System Sanitation: Executed a clean-slate Windows 11 Pro deployment to eliminate legacy driver conflicts and kernel-level errors.
Firmware Configuration: Optimized BIOS/UEFI settings to enable Intel VT-x, providing the necessary hardware-abstraction layer for both WSL 2 and VirtualBox.

Phase 2: Native Kernel Integration (WSL 2)
Backend Initialization: Utilized the Windows Terminal to enable the Virtual Machine Platform and Windows Subsystem for Linux features.
Environment Deployment: Successfully deployed Ubuntu 24.04 LTS via the native WSL 2 architecture.
Verification: Configured UNIX user credentials and verified shell accessibility, establishing a stable CLI-based Linux environment directly integrated with the Windows host.

Phase 3: Full Virtualization & Security Hardening (VirtualBox)
Hypervisor Setup: Configured a dedicated VirtualBox instance with 25GB of allocated storage for Ubuntu 24.04.3 LTS.
CLI Troubleshooting: Resolved a graphical installer hang during the Ubuntu Pro setup by pivoting to the terminal to manually finalize registration.

Enterprise Integration:
Manually attached the system to Ubuntu Pro using a personal token via terminal.
Enabled ESM (Expanded Security Maintenance) and Livepatch for continuous security patching.
Successfully executed a 105.4 MB system update cycle through the Software Updater.

Phase 4: Workspace & Display Optimization
Driver Integration: Installed VirtualBox Guest Additions to enable bidirectional clipboard support and advanced graphics handling.
Display Mapping: Corrected initial scaling issues and "letterboxing" by configuring a hardware-matched resolution of 1920x1080 in Full-Screen mode.

## Key Findings
Technical Integrity: Proved that a clean-slate deployment is the only reliable method for ensuring 100% compatibility between hardware and multiple virtualized kernels.
CLI Dependency: Confirmed that terminal proficiency is essential for bypassing GUI failures in enterprise-grade Linux distributions.
Efficiency: Identified that a total system "rebuild" is often faster and more stable than troubleshooting fragmented legacy environments.

## Outcomes
Operational Readiness: Established two distinct, high-performance Linux environments (Native WSL 2 and Virtualized VirtualBox) running simultaneously on a single host.
SOP Validation: Developed a repeatable, standardized process for workstation recovery and environment deployment.
