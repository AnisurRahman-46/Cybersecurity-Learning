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
 ## We will learn how to create a Directory in Kali Linux using these basic commands. 

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

🔹 Step 1: Open Terminal
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

