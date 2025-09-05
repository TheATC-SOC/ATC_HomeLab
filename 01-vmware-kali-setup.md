Date: Sept 9, 2025

🎯 Objective

The goal of this project was to establish the foundation of my personal cybersecurity homelab. I achieved this by installing VMware Workstation as the hypervisor and deploying Kali Linux as my primary attacker machine. This environment will serve as the baseline for future labs involving penetration testing, SOC/SIEM monitoring, and red-team vs. blue-team simulations.

🛠️ Tools & Technology
Component	Purpose
VMware Workstation 17	Hypervisor for creating and managing virtual machines
Kali Linux (VMware Image)	Attacker machine with pre-installed security tools
7-Zip	Utility to extract Kali’s compressed VM archive
Local Storage (80 GB)	Disk allocation for VM images and snapshots
4 GB RAM / 4 CPU Cores	Optimized system resources dedicated to Kali
👣 Steps Taken
🔹 Step 1: Download VMware Workstation

Registered for a Broadcom account.

Navigated to Free Downloads → VMware Workstation Pro and downloaded version 17.6.4.

📸 Screenshot:

<img width="1387" height="1103" alt="free downloads" src="https://github.com/user-attachments/assets/a4dd13c8-5d31-49de-aab0-67129c0314d9" />

🔹 Step 2: Install 7-Zip

Downloaded 7-Zip from the official site.

Installed it to handle .7z compressed files.

Used it to extract Kali’s pre-built VM package.

📸 Screenshot:

<img width="1504" height="879" alt="7zip" src="https://github.com/user-attachments/assets/83613ce2-c0d1-45cd-b575-79308f111030" />

🔹 Step 3: Download Kali Linux Pre-Built VM

Went to Kali’s official site.

Selected Pre-Built Virtual Machine → VMware for faster setup.

Extracted the .7z archive with 7-Zip.

📸 Screenshots:

<img width="1589" height="1106" alt="Screenshot 2025-09-05 101123" src="https://github.com/user-attachments/assets/d0dc4890-b6c1-4c74-a639-3d72d456c940" />

<img width="1215" height="710" alt="Screenshot 2025-09-05 101550" src="https://github.com/user-attachments/assets/f79dedb0-a093-4dc0-97fc-1bdc7f0e89bc" />

🔹 Step 4: Import Kali VM into VMware

Opened VMware Workstation Player.

Selected Open a Virtual Machine.

Loaded the extracted .vmx file into the library.

📸 Screenshot:

<img width="743" height="612" alt="openVM" src="https://github.com/user-attachments/assets/498bae50-b37f-40ad-bb83-aa2c79a04edb" />

🔹 Step 5: Boot Kali Linux

Started the VM successfully.

Logged in using the default credentials:

Username: kali

Password: kali

📸 Screenshot:

<img width="743" height="611" alt="openVM3" src="https://github.com/user-attachments/assets/4fb926d4-7dd4-41bc-978b-55f186c7ce60" />

🔹 Step 6: Configure VM Settings

To improve performance, I customized the VM resources:

Memory: 4 GB (recommended 2 GB, minimum 1 GB)

Processors: 4

Hard Disk: 80 GB

Network Adapter: NAT

This configuration ensures smoother performance and supports multitasking when running penetration testing tools.

📸 Screenshot:

<img width="755" height="733" alt="virtual_machine_setting" src="https://github.com/user-attachments/assets/b39a5b8b-7890-4663-a118-c823214d82c6" />

✅ Result

VMware Workstation installed successfully.

Kali Linux VM imported and running.

Verified desktop environment access.

Resources optimized for better stability and performance.

🚀 Next Steps

Increase VM resources if more performance is required.

Create a second VM (Windows or Ubuntu) to act as a target machine.

Configure a virtual network for attacker/defender simulations.

Document penetration testing exercises and SOC-style monitoring with tools like Splunk or Wireshark.


