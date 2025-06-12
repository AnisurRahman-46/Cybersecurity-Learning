# 🔧 Create a Custom `myip` Command to Show Only eth0 IP Address

So, in the previous class, we learned about the `ifconfig` command, which is commonly used in Kali Linux. When we run ifconfig, we get a lot of unnecessary output, especially under the `eth0` section

![image](https://github.com/user-attachments/assets/3b11b599-33d5-4c9c-955d-4ebbf059da93)

> **_Among that, we get a finite value next to `inet`, which is the IP address. Along with the IP address, we also get many other unwanted details.
So, today we will create our own *custom command* to display only the IP address._**

---

This guide explains how to create a custom shell command called `myip` in Kali Linux that will display only the system's IP address from the `eth0` interface.

---

## 🪜 Step-by-Step Instructions:

### 🔹 Step 1: Create a new directory

Use the `mkdir` command to create a new folder for your project.

```
mkdir mycode
```
---

### 🔹 Step 2: Change into that directory

Use the `cd` command to move into the newly created folder:

```
cd mycode/
```
---

### 🔹 Step 3: Create a shell script file

Create a new shell script file using `nano`:

```
nano myip.sh
```
> Here .sh -> Bash File. (Just like we use .py extention for Python)

---

### 🔹 Step 4: Paste the following code inside `myip.sh`

```
ifconfig eth0 | grep inet | grep -v ":" | awk '{print $2}'
```
![saving file](https://github.com/user-attachments/assets/14ac0889-9a0e-4bb0-a010-fc9b3bab5c94)

---

### 🔹 Step 5: Save and exit the nano editor

- Press `CTRL + O` to save the file
- Press `Enter` to confirm the filename
- Press `CTRL + X` to exit

Now your script file `myip.sh` has been created.

---

### 🔹 Step 6: Make the script executable

Give execute permission to the script using `chmod`:

```
chmod +x myip.sh
```
> 💡 **Why do we give execute permission?**  
>
> When we first create the file, its default permissions may look something like this:
>
> ```
> -rw-rw-r-- 1 kali kali 59 Jun  7 08:48 myip.sh
> ```
>
> Here:
> - `r` = read permission
> - `w` = write permission
> - `x` = execute permission
>
> As you can see, there is **no `x` (execute)** permission by default.  
> That's why we run:
>
> ```
> chmod +x myip.sh
> ```
>
> This command gives the file **permission to be executed as a script**.  
> After that, the permissions change to:
>
> ```
> -rwxrwxr-x 1 kali kali 59 Jun  7 08:48 myip.sh
> ```
>
> Now the file can be run using:
>
> ```
> ./myip.sh
> ```

---

### 🔹 Step 7: List files to confirm permission

Use the `ls -l` command to check that the file has executable (`x`) permission:

```
ls -l
```
---

### 🔹 Step 8: Run the script

Execute the script using:

```
./myip.sh
```

It will show output like:

```
192.168.1.15
```
**_But here we don't want to write `./myip.sh`, We want to simply give `myip` command to get the result._**

---

### 🔹 Step 9: Move Script to a System-Wide Path

For that we will use another command `mv`
```
mv myip.sh myip
```
> - The first part (`myip.sh`) is the **current file name**.
> - The second part (`myip`) is the **new name** you want to give it.
---

### 🔹 Step 10: Move the script to a system-wide location

To make the `myip` command accessible from **anywhere** in the terminal (without using `./`), move the script to the `/usr/local/bin/` directory:

```
sudo mv myip.sh /usr/local/bin/myip
```

> 🔒 Note: We're also renaming the file to just `myip` (no `.sh`) for simplicity.

---

### 🔹 Step 11: Test your custom command

Now that the script is in your system path, you can simply run:

```
myip
```

**Expected Output**:

```
192.168.56.142
```
---

**_And done! We have created our custom command of `myip` by which typing a simple word we can get the `inet` (IP Address) value without getting unnecessary details._**

---
