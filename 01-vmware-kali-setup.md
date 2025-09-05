Project 01 – VMware + Kali Linux Setup

Date: Sept 9, 2025

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

<img width="1387" height="1103" alt="free downloads" src="https://github.com/user-attachments/assets/a4dd13c8-5d31-49de-aab0-67129c0314d9" />




<img width="1610" height="913" alt="Screenshot 2025-09-05 100733" src="https://github.com/user-attachments/assets/a614928c-2565-47e8-80a3-4b88158decd9" />



🔹 Step 2: Install 7-Zip (to Extract Kali Files)

Downloaded 7-Zip from official site.

<img width="1504" height="879" alt="7zip" src="https://github.com/user-attachments/assets/701e584a-e4c8-4397-b7cc-77235662564d" />


Used it to unpack the .7z Kali VM archive.


🔹 Step 3: Download Kali Linux Pre-Built VM

From Kali’s official site, selected Pre-Built Virtual Machine → VMware.

<img width="1215" height="710" alt="Screenshot 2025-09-05 101550" src="https://github.com/user-attachments/assets/8f19e622-ecd9-4c95-99dc-0fbd422cef77" />


Extracted the .7z archive with 7-Zip.


🔹 Step 4: Import Kali VM into VMware

Opened VMware Workstation Player.

<img width="743" height="612" alt="openVM" src="https://github.com/user-attachments/assets/c6656384-18ac-4d4b-8a1e-cc16606e51fa" />


Selected Open a Virtual Machine.

Loaded the .vmx file.


🔹 Step 5: Boot Kali Linux

Started the VM.

<img width="743" height="611" alt="openVM3" src="https://github.com/user-attachments/assets/9d4f901e-4ae2-4e0c-8f61-00b3be98029d" />

Logged in with default credentials:

Username: kali

Password: kali


🔹 Step 6: Configure VM Settings

After importing Kali, I adjusted the VM resources for better performance:

<img width="755" height="733" alt="virtual_machine_setting" src="https://github.com/user-attachments/assets/5bc6f2d8-8fe8-4b24-bc89-eebe43b189e4" />


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
