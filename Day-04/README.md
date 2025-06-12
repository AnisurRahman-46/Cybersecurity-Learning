# 📦 Basic Linux Commands for Beginners

Welcome to the **Linux Basic Commands** guide. Here you will learn some of the most commonly used Linux terminal commands — explained simply with examples!

---

## 📁 File & Directory Commands

| Command  | Description                      | Example                         |
|:---------|:---------------------------------|:--------------------------------|
| `ls`     | List files and folders           | `ls`                            |
| `cd`     | Change directory                 | `cd Desktop`                    |
| `pwd`    | Show current directory path      | `pwd`                           |
| `mkdir`  | Make a new directory             | `mkdir newfolder`               |
| `rmdir`  | Remove an empty directory        | `rmdir newfolder`               |
| `touch`  | Create an empty file             | `touch notes.txt`               |
| `rm`     | Remove file or folder            | `rm notes.txt` / `rm -r folder` |
| `cp`     | Copy file or folder              | `cp file1.txt file2.txt`        |
| `mv`     | Move or rename files             | `mv file1.txt folder/`          |

---

## 📖 Help & Permissions Commands

| Command      | Description                     | Example                         |
|:-------------|:--------------------------------|:--------------------------------|
| `man`        | Show manual for a command       | `man ls`                        |
| `echo`       | Print message to terminal       | `echo "Hello World"`            |
| `chmod`      | Change file permissions         | `chmod 755 script.sh`           |
| `chown`      | Change file owner and group     | `sudo chown user file.txt`      |

---

## ⚙️ System & Process Commands

| Command      | Description                     | Example               |
|:-------------|:--------------------------------|:----------------------|
| `ps`         | Show running processes          | `ps aux`              |
| `kill`       | Kill a running process          | `kill 1234`           |
| `top`        | Live system processes summary   | `top`                 |
| `df`         | Check disk space usage          | `df -h`               |
| `du`         | Check folder/file size          | `du -h file.txt`      |

---

## 📑 File Viewing & Editing Commands

| Command      | Description                   | Example                   |
|:-------------|:------------------------------|:--------------------------|
| `cat`        | Display file content          | `cat file.txt`            |
| `nano`       | Open nano text editor         | `nano file.txt`           |
| `vi`         | Open vi text editor           | `vi file.txt`             |

---

## 🧹 Miscellaneous Commands

| Command      | Description                     | Example    |
|:-------------|:--------------------------------|:-----------|
| `clear`      | Clear the terminal screen       | `clear`    |
| `exit`       | Close the terminal              | `exit`     |

---

## ✅ Note  
These are the most common commands every Linux beginner should know. Practice them daily to get comfortable in the terminal environment!

---
 ## We will learn how to create a _Directory_ in Kali Linux using these basic commands. 

 ### 📂 Step 1: List Existing Files and Folders
 
Use `ls` to see what's already in the current directory.
```
ls
```
📌 Example output:

Documents  Downloads  Music  Pictures

 ### 🆕 Step 2: Create a New Directory
 
Use `mkdir` followed by the name of the folder you want to create.
```
mkdir cybersec-notes
```
✅ This creates a directory called **Cybersec-notes** in the current location.

### 📁 Step 3: Verify the Directory Was Created

Use `ls` again to check if the new folder is listed.
```
ls
```
📌 Example output:

cybersec-notes Documents  Downloads  Music  Pictures 

### 🔄 Step 4: Change Into the New Directory

Use `cd` to move into the new directory.
```
cd cybersec-notes
```
✅ Now you're inside the myproject folder.

### 📍 Step 5: Confirm Your New Location

Use `pwd` again to confirm you're in the right place.
```
pwd
```
📌 Example output:

/home/kali/cybersec-notes

*_Now we have created our own Directory in Kali Linux._* 
---
---


# 👤 Create a New User in Kali Linux

🔹 Step 1: Open Terminal: 
Open the terminal in Kali Linux.

🔹 Step 2: Create a New User
```
sudo adduser <username>
```
Add any username like John, Alice etc. 

🔹 Step 3: Set or Change the User’s Password
```
sudo passwd <username>
```
🔹 Step 4: Add User to a Group
```
sudo usermod -aG sudo <username>
```

🔹 Step 5: Done! Test the New User
Switch to the new user:
```
su - <username>
```
---

# 🧰 Let's Learn some more useful commands of Kali Linux

This document explains some essential Linux system monitoring and networking commands with example usage and readable output. These are commonly used in Kali Linux 

---

## 1. 📦 Disk Space Usage: `df -h`

**Description**:
Displays disk space usage for all mounted filesystems in **human-readable** format.

**Command**:

```
df -h
```
**Example Output**: 

![image](https://github.com/user-attachments/assets/680c6041-4fad-4c46-89f3-9e8a3f5a7aed)

---

## 2. 🧠 System Monitor: htop

**Description**:
An interactive process viewer (like Task Manager) to monitor CPU, memory, and running processes.

**Command**:
```
htop
```
**Example Output** : 

![image](https://github.com/user-attachments/assets/bae4518b-65d2-4a25-b196-3fddb85eadc8)

---

## 3. 🌐 View Network Interfaces: ifconfig

**Description**:
Displays all network interfaces and their IP addresses.

**Command**:
```
ifconfig
```
**Example Output**:

eth0: flags=4163<UP,BROADCAST,RUNNING>  mtu 1500
        inet 192.168.1.10  netmask 255.255.255.0  broadcast 192.168.1.255
        ...
        
🛠️ If ifconfig is not found, **_install_**  it via:
```
sudo apt install net-tools
```
---

That's all for today's Learning. Do revise everything once more and most importantly **Practice** by yourself again and again. Let's move to our Day-05 (https://github.com/AnisurRahman-46/Cybersecurity-Learning/tree/main/Day-05)

---
