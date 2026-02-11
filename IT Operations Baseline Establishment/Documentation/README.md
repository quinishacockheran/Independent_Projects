# IT Operations: Baseline Establishment
By Quinisha Cockheran   

## Executive Summary
This project details the systematic re-engineering of a primary workstation to serve as a high-performance laboratory for CompTIA A+ simulations and multi-OS experimentation. Following a critical failure of secondary kernel integration (WSL 2), a strategic decision was made to execute a full system recovery. This ensured a "Pristine State" baseline, optimized for virtualization, secure sandboxing, and cross-platform development.   

## Purpose
The objective of this deployment was to move beyond a standard "daily-use" configuration into a dedicated IT Operations environment. By establishing a clean hardware-software baseline, this project ensures 100% compatibility for advanced hypervisor testing and custom disk partitioning, reducing future technical debt and troubleshooting overhead.   

## Tools Used
- Windows 11 Pro - Host Operating System and primary administrative environment
- Windows Media Creation Tool - For clean-slate OS deployment and storage sanitation
- Disk Management/DiskPart - For strategic partition allocation and unallocated space reservation
- BIOS/UEFI Firmware - Hardware-level optimization for virtualization (Intel VT-x)
- GitHub - For version control and Technical SOP documentation

## Methodology
**Infrastructure Audit & Incident Identification**
- Identified persistent kernel-level initialization errors within the existing WSL 2 environment
- Determined that legacy system files and partition fragmentation were the root causes of the suboptimal baseline

**Storage Sanitation & OS Deployment**
- Allocated primary partitions for the host OS while maintaining a clean, single-volume baseline to maximize resources for Type-2 Hypervisors.
- Prepared hardware-level virtualization settings (Intel VT-x) to support a dual-layer Linux environment: WSL 2 for CLI proficiency and VirtualBox for full GUI experimentation.

**Strategic Partitioning & Virtualization Prep**
- Allocated primary partitions for the host OS while strategically reserving unallocated space for future Linux (dual-boot) integration
- Configured hardware-level virtualization settings to support future Type-2 hypervisor labs

**Validation & Documentation**   
- Verified system stability and baseline performance
- Developed this Technical SOP to document the recovery process and establish a repeatable deployment standard

## Key Findings (Lessons Learned)
- Strategic Pivoting: In technical operations, identifying the point where "repair" becomes less efficient than "rebuild" is critical for maintaining project timelines
- Environment Isolation: A clean-slate deployment is the only way to ensure 100% hardware-software compatibility for high-level virtualization labs
- Documentation Value: Establishing a baseline recovery SOP saves hours of future debugging by providing a known, stable starting point

## Outcomes
- A functional, high-performance IT Lab environment ready for CompTIA A+ simulations  
- A standardized "Fresh Start" deployment manual for future workstation re-engineering
- Successfully integrated host-level and kernel-level stability for cross-platform experimentation
