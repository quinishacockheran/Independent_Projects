# IT Operations: Baseline Establishment
*By Quinisha Cockheran*

## Executive Summary
This project details the systematic re-engineering of a primary workstation to serve as a high-performance laboratory for CompTIA A+ simulations and multi-OS experimentation[cite: 2]. Following a critical failure of secondary kernel integration (WSL 2), a strategic decision was made to execute a full system recovery[cite: 3, 5]. This ensured a "Pristine State" baseline, optimized for virtualization, secure sandboxing, and cross-platform development[cite: 2, 7].

## Purpose
The objective of this deployment was to move beyond a standard "daily-use" configuration into a dedicated IT Operations environment[cite: 6]. By establishing a clean hardware-software baseline, this project ensures 100% compatibility for advanced hypervisor testing and custom disk partitioning—reducing future technical debt and troubleshooting overhead[cite: 7, 12].

## Tools Used
- **Windows 11 Pro** - Host Operating System and primary administrative environment[cite: 9].
- **Windows Media Creation Tool** - For clean-slate OS deployment and storage sanitation[cite: 8, 9].
- **Disk Management / DiskPart** - For strategic partition allocation and unallocated space reservation[cite: 10].
- **BIOS/UEFI Firmware** - Hardware-level optimization for virtualization (Intel VT-x/AMD-V).
- **GitHub** - For version control and Technical SOP documentation[cite: 1].

## Methodology
1. **Infrastructure Audit & Incident Identification**
   - Identified persistent kernel-level initialization errors within the existing WSL 2 environment[cite: 3].
   - Determined that legacy system files and partition fragmentation were the root causes of the suboptimal baseline[cite: 4].

2. **Storage Sanitation & OS Deployment**
   - Executed a full drive wipe to eliminate legacy partition tables and potential software conflicts[cite: 8].
   - Clean-installed Windows 11 Pro from verified external boot media to ensure system integrity[cite: 9].

3. **Strategic Partitioning & Optimization**
   - Allocated primary partitions for the host OS while strategically reserving unallocated space for future Linux (dual-boot) integration[cite: 10].
   - Configured hardware-level virtualization settings to support future Type-2 hypervisor labs.

4. **Validation & Documentation**
   - Verified system stability and baseline performance.
   - Developed this Technical SOP to document the recovery process and establish a repeatable deployment standard[cite: 11, 12].

## Key Findings (Lessons Learned)
- **Strategic Pivoting:** In technical operations, identifying the point where "repair" becomes less efficient than "rebuild" is critical for maintaining project timelines[cite: 11].
- **Environment Isolation:** A clean-slate deployment is the only way to ensure 100% hardware-software compatibility for high-level virtualization labs[cite: 7].
- **Documentation Value:** Establishing a baseline recovery SOP saves hours of future debugging by providing a known, stable starting point[cite: 12].

## Outcomes
- A functional, high-performance IT Lab environment ready for CompTIA A+ simulations.
- A standardized "Fresh Start" deployment manual for future workstation re-engineering.
- Successfully integrated host-level and kernel-level stability for cross-platform experimentation.
