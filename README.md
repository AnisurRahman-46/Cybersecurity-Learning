# Cybersecurity-Learning
# Cybersecurity Learning Journey with Anisur

Welcome to my **Cybersecurity Journey Repository**!  
This repository is created and maintained by **Anisur Rahman** to document everything I learn in the field of **Cybersecurity** — including Ethical Hacking, Networking, Penetration Testing, and more.

I will regularly update this repo with notes, resources, tools, and tips to help anyone starting their journey in cybersecurity.

---

# 🔥 Kali Linux Setup on VirtualBox — Step by Step

- Suggestion - Read all the steps first then follow it for better clarification about every step. 

## 📦 Requirements

1. [VirtualBox Download (for Windows/Linux/Mac)](https://www.virtualbox.org/wiki/Downloads)
2. [Kali Linux (VirtualBox Image)](https://www.kali.org/get-kali/#kali-virtual-machines)
3. [7-Zip Download (for Windows)](https://www.7-zip.org/download.html)

---

## 📥 Download & Installations

### 📌 1️⃣ Install VirtualBox:
- Go to the [VirtualBox Downloads](https://www.virtualbox.org/wiki/Downloads)
- Download according to your OS (Windows / macOS / Linux)
- Install the setup normally like any other software.

---

### 📌 2️⃣ Install 7-Zip:
- Download the latest `.exe` setup from [7-Zip Downloads](https://www.7-zip.org/download.html)
- Install it (simple next-next-finish)

---

### 📌 3️⃣ Download Kali Linux for VirtualBox:
- Visit [Kali Virtual Machines](https://www.kali.org/get-kali/#kali-virtual-machines)
- Under **Kali Linux VirtualBox Images**, download the latest `.7z` file.

---

## 📦 Extract Kali Linux Image using 7-Zip

- Go to the folder where you downloaded the `.7z` Kali Linux file.
- **Right click on the file → 7-Zip → Extract to 'filename/'**
  
  (Best practice — use `Extract to 'kali-linux-xxx/'` so files stay organized)
  
  (After Extraction it may not be visible at the top so don't get panic. Just Scroll down observing Properly, 100% it will be there.)

---

## 📤 Import Kali Linux into VirtualBox

- NOTE: After Setting Up all the applications and files. You can Simply click the folder of Kali Linux and double click on a blue box named as (eg. Kali.Linux-2025 ...) as shown below.
- ![image](https://github.com/user-attachments/assets/e6ee7d88-8584-426e-a032-8f14a2753b73)
  Double Click the Blue Box and it will automatically be set up in the Virtual Box.

  OR you can follow the below mentioned steps.
 
1. Open **VirtualBox**
2. Click on `File` → `Import Appliance`
3. Browse to the extracted `.ova` file (inside the extracted Kali folder)
4. Click `Next` → Review settings
5. Click `Import`

---

## ⚙️ Adjust VM Specifications (Optional but Recommended)

- Select your **Kali VM** in VirtualBox
- Click `Settings`
- Go to `System` tab
  - Increase **Base Memory** (e.g., 2048 MB or 4096 MB if available)
- Go to `Processor` tab
  - Increase to 2 CPUs if your system allows.
- Go to `Display` tab
  - Increase `Video Memory` to at least 64 MB.

---

## 🚀 Start Kali Linux VM

- Select the imported Kali VM
- Click `Start`
- Done ✅

---

## 📌 Notes:

- Download **Kali VirtualBox Image**, not VMware one.
- `.7z` files need **7-Zip** to extract, Windows built-in extractor won’t work.
- Keep extracted files organized in one folder.
- Adjust specifications based on your laptop’s available RAM and CPU.









