# 🎯 Objective

The goal of this project is to establish the foundation of my personal cybersecurity homelab. I achieved this by installing VMware Workstation as the hypervisor and deploying Kali Linux as my primary attacker VM.

---

# 🛠️ Tools & Technology

## Host System Requirements

- A computer running Windows (or Linux/macOS if supported by VMware Workstation)
- Administrative privileges on the host machine 

## Hardware Minimums

- At least 4 GB RAM (preferably 8 GB or more for smoother performance)
- At least 4 CPU cores
- 80 GB free disk space (for VM images and snapshots)

## Software & Accounts

- Broadcom Account (required to download VMware Workstation Pro)
- VMware Workstation 17.x installer (downloaded from Broadcom/VMware website)
- 7-Zip utility (for extracting compressed VM files)
- Kali Linux Pre-Built VMware image (downloaded from the official Kali website)
- Internet Connection (stable internet access to download software and OS images)
- Optional: 
  - Secondary VM image (Windows or Ubuntu) for target machine scenarios
  - External storage for backups/snapshots

---

# 👣 Steps Taken

## Step 1. Download VMware Workstation

1. Register for a Broadcom account.
2. Navigate to Free Downloads → VMware Workstation Pro and download version 17.6.4.

📸 Screenshot:

<img width="1387" height="1103" alt="free downloads" src="https://github.com/user-attachments/assets/a4dd13c8-5d31-49de-aab0-67129c0314d9" />

## Step 2. Install 7-Zip

1. Download 7-Zip from the official site.
2. Install it to handle .7z compressed files.
3. Use it to extract Kali’s pre-built VM package.

📸 Screenshot:

<img width="1504" height="879" alt="7zip" src="https://github.com/user-attachments/assets/83613ce2-c0d1-45cd-b575-79308f111030" />

## Step 3. Download Kali Linux Pre-Built VM

1. Go to Kali’s official site.
2. Select Pre-Built Virtual Machine → VMware for faster setup.
3. Extract the .7z archive with 7-Zip.

📸 Screenshots:

<img width="1589" height="1106" alt="Screenshot 2025-09-05 101123" src="https://github.com/user-attachments/assets/d0dc4890-b6c1-4c74-a639-3d72d456c940" />

<img width="1215" height="710" alt="Screenshot 2025-09-05 101550" src="https://github.com/user-attachments/assets/f79dedb0-a093-4dc0-97fc-1bdc7f0e89bc" />

## Step 4. Import Kali VM into VMware

1. Open VMware Workstation Player.
2. Select "Open a Virtual Machine."
3. Load the extracted `.vmx` file into the library.

📸 Screenshot:

<img width="743" height="612" alt="openVM" src="https://github.com/user-attachments/assets/498bae50-b37f-40ad-bb83-aa2c79a04edb" />

## Step 5. Boot Kali Linux

1. Start the VM successfully.
2. Log in using the default credentials:

   - Username: kali
   - Password: kali

---

## 🔒 Changing the Default Kali Linux Password

It’s important to change the default password (`kali`) immediately after your first login to secure your homelab environment.

### Steps to Change Your Password

1. **Open Terminal in Kali Linux.**
2. **Run the password change command:**
   ```bash
   passwd
   ```
3. **Enter your current password when prompted:**
   ```
   Current password: kali
   ```
4. **Enter your new password twice to confirm:**
   ```
   New password: [your_new_password]
   Retype new password: [your_new_password]
   ```
5. **Success message should appear:**
   ```
   passwd: password updated successfully
   ```

#### Tips

- Choose a strong password (at least 8 characters, mix of letters, numbers, symbols).
- Write your new password down or store it in a password manager.
- You can change passwords for other users by running:
  ```bash
  sudo passwd [username]
  ```

**Reference:**  
- [Kali Linux User Guide – Managing User Accounts](https://www.kali.org/docs/general-use/user-management/)

📸 Screenshot:

<img width="743" height="611" alt="openVM3" src="https://github.com/user-attachments/assets/4fb926d4-7dd4-41bc-978b-55f186c7ce60" />

---

## Step 6. Configure VM Settings

1. To improve performance, customize the VM resources:
   - Memory: 4 GB (recommended 2 GB, minimum 1 GB)
   - Processors: 4
   - Hard Disk: 80 GB
   - Network Adapter: NAT

This configuration ensures smoother performance and supports multitasking when running penetration testing tools.

📸 Screenshot:
<img width="755" height="733" alt="virtual_machine_setting" src="https://github.com/user-attachments/assets/b39a5b8b-7890-4663-a118-c823214d82c6" />

---

# 🐞 Troubleshooting

- **VM Won’t Boot:**  
  Confirm your hardware meets requirements and that virtualization is enabled in BIOS/UEFI.

- **Network Issues:**  
  Make sure your VM network adapter is set to NAT or Bridged. Restart the VM after making changes.

- **Login Problems:**  
  Double-check default credentials. If you changed the password and forgot it, you may need to re-import the VM or reset the password.

---

# ✅ Result

- VMware Workstation installed successfully.
- Kali Linux VM imported and running.
- Verified desktop environment access.
- Resources optimized for better stability and performance.

---

# 🚀 Next Steps

1. **Increase VM resources** if more performance is required.
   - Adjust RAM, CPU, or disk allocations in VMware settings.

2. **Create a second VM (Windows or Ubuntu) to act as a target machine.**
   - Download pre-built images from official sources and repeat the import steps above.

3. **Configure a virtual network for attacker/defender simulations.**
   - Explore VMware’s virtual networking options or follow guides like [VMware Networking Explained](https://docs.vmware.com/en/VMware-Workstation-Pro/17.0/com.vmware.workstation.using.doc/GUID-6C3E81E5-4EBA-4E3E-9B38-CCF8A9E7F7D0.html).

4. **Document penetration testing exercises and SOC-style monitoring with tools like Splunk or Wireshark.**
   - Consider keeping a lab journal or repository for your exercises and findings.

---

# 🧩 Why This Stack?

- **VMware Workstation:** Reliable hypervisor, widely used in both enterprise and personal labs. It supports a broad range of guest operating systems and offers robust performance and snapshot capabilities for easy backup and recovery.
- **Kali Linux:** The industry standard for penetration testing, red teaming, and offensive security training. Comes pre-installed with hundreds of security tools and is well-documented for beginners and professionals.
- **7-Zip:** Free, open-source utility for extracting compressed files, often required for downloadable VM images.

---

# 🌐 Useful Resources

- [Kali Linux Documentation](https://www.kali.org/docs/)
- [VMware Workstation Pro Documentation](https://docs.vmware.com/en/VMware-Workstation-Pro/index.html)
- [7-Zip Official Site](https://www.7-zip.org/)
- [Kali Linux Pre-Built VMware Images](https://www.kali.org/get-kali/#kali-virtual-machines)
- [Broadcom VMware Account Registration](https://customerconnect.vmware.com/)
- [YouTube: Setting Up VMware Workstation](https://www.youtube.com/results?search_query=vmware+workstation+setup)
- [YouTube: Installing Kali Linux on VMware](https://www.youtube.com/results?search_query=install+kali+linux+vmware)
