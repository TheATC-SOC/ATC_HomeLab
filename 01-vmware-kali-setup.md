Project 01 – VMware + Kali Linux Setup

Date: Sept 9, 2025
Created by: Wonhee Oh

Objective

Set up the foundation of my cybersecurity homelab by installing VMware Workstation and deploying Kali Linux. This environment will be used for penetration testing, SOC/SIEM experiments, and future red-team vs blue-team labs.

Tools & Technology
Component	Purpose
VMware Workstation 17	Hypervisor for running VMs
Kali Linux (VMware)	Attacker machine with pre-installed security tools
7-Zip	Tool for extracting Kali Linux VM archive
Local Storage (80 GB)	Disk allocation for VM
4 GB RAM / 4 CPU cores	VM resource allocation

Steps Taken

🔹 Step 1: Download VMware Workstation

Registered for a Broadcom account.

Navigated to Free Downloads → VMware Workstation Pro.


🔹 Step 2: Install 7-Zip (to Extract Kali Files)

Downloaded 7-Zip from official site.

Used it to unpack the .7z Kali VM archive.


🔹 Step 3: Download Kali Linux Pre-Built VM

From Kali’s official site, selected Pre-Built Virtual Machine → VMware.

Extracted the .7z archive with 7-Zip.


🔹 Step 4: Import Kali VM into VMware

Opened VMware Workstation Player.

Selected Open a Virtual Machine.

Loaded the .vmx file.


🔹 Step 5: Boot Kali Linux

Started the VM.

Logged in with default credentials:

Username: kali

Password: kali


🔹 Step 6: Configure VM Settings

After importing Kali, I adjusted the VM resources for better performance:

Memory: 4 GB (recommended 2 GB, minimum 1 GB)

Processors: 4

Hard Disk: 80 GB

Network Adapter: NAT

This ensures Kali runs smoothly and allows for multitasking when running penetration testing tools.

Result

✅ VMware Workstation installed successfully
✅ Kali Linux VM running inside VMware
✅ Verified access to full Kali desktop environment
✅ Resources optimized (CPU/RAM/Storage)



Next Steps

Increase VM resources further if needed.

Create a second VM (Windows/Ubuntu) as a target machine.

Configure network settings for attack/defense labs.

Document penetration testing exercises.
