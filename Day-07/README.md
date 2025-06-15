# 📖 NMap Learning Repository

Today we will be learning about **NMap** — which is a powerful open-source network scanning tool. First we will make a `nmap` directory, then we will move to it and then we will learn about commonly used NMap commands. 

---

## 📂 How to Make NMap Directory & Navigate Inside  

### 📌 Step 1: Make Directory  

We will use `mkdir` command to make a directory.
```
mkdir nmap
```

### 📌 Step 2: Move to the Directory 

We will use `cd` command to move to our nmap directory.
```
cd nmap
```

> Now as we have learnt to create `nmap` directory, we will be learning about different type of NMap commands.


---

# 🛠️ NMap Commands

### 1. TARGET SPECIFICATION:

  -iL <inputfilename>: Input from list of hosts/networks

---

### 2. HOST DISCOVERY:

  -sL: List Scan - simply list targets to scan
  -sn: Ping Scan - disable port scan
  -Pn: Treat all hosts as online -- skip host discovery

---

### 3. SCAN TECHNIQUES:

  -sS/sT/sA: TCP SYN/Connect()/ACK
  -sU: UDP Scan

---

### 4. PORT SPECIFICATION AND SCAN ORDER:

  -p <port ranges>: Only scan specified ports
    Ex: -p22; -p1-65535; -p U:53,111,137,T:21-25,80,139,8080,S:9

  --exclude-ports <port ranges>: Exclude the specified ports from scanning
  -F: Fast mode - Scan fewer ports than the default scan
  -r: Scan ports sequentially - don't randomize

---

### 5. SERVICE/VERSION DETECTION:

  -sV: Probe open ports to determine service/version info
  --version-intensity <level>: Set from 0 (light) to 9 (try all probes)
  --version-light: Limit to most likely probes (intensity 2)
  --version-all: Try every single probe (intensity 9)
  --version-trace: Show detailed version scan activity (for debugging)

---

### 6. SERVICE/VERSION DETECTION:

  -sV: Probe open ports to determine service/version info
  --version-intensity <level>: Set from 0 (light) to 9 (try all probes)
  --version-light: Limit to most likely probes (intensity 2)
  --version-all: Try every single probe (intensity 9)
  --version-trace: Show detailed version scan activity (for debugging)

---

### 7. TIMING AND PERFORMANCE:

  -T<0-5>: Set timing template (higher is faster)
  --scan-delay/--max-scan-delay <time>: Adjust delay between probes
  --min-rate <number>: Send packets no slower than <number> per second
  --max-rate <number>: Send packets no faster than <number> per second

---

### 8. OS DETECTION:

  -O: Enable OS detection

---

### 9. OUTPUT:

  -oN/-oX/-oS/-oG <file>: Output scan in normal txt, XML
  -v: Increase verbosity level (use -vv or more for greater effect)

  -v: [Level 1]
  -vv: [Level 2 report of real time scan] - Recommended
  -vvv: [Level 3 report of real time scan]

---

### 10. MISC:

  -A: Enable OS detection, version detection, script scanning, and traceroute

---

Now as we completed about Nmap and it's commands, we will be moving to gain some insight about **_Docker_**. 

---

# 📦 Docker and It's Use in Cybersecurity

## 📌 What is Docker?

Docker is an **open-source platform** designed to automate the deployment, scaling, and management of applications using lightweight, portable containers.

A **Docker container** packages an application and all its dependencies (libraries, system tools, code, and runtime) so it runs consistently across different computing environments.

---

## 📌 Why Do We Use Docker?

- To avoid the "It works on my machine!" problem.
- To run isolated environments for testing and analysis.
- To easily replicate, deploy, and scale apps in controlled, reproducible containers.
- To save system resources compared to virtual machines.

---

## 📌 Where Do We Use Docker in Cybersecurity?

Docker is heavily used in cybersecurity for:

- **Sandboxing malware** in isolated containers for safe analysis.
- Creating **temporary penetration testing labs**.
- Deploying tools like **Kali Linux Docker images** or **security scanners** without affecting the host OS.
- Quickly setting up **CTFs (Capture The Flag) and challenges** environments.
- Running web apps to test against vulnerabilities like SQL Injection, XSS, etc.

---

## 📌 When and How to Use Docker?

**When:**
- When you need an isolated, controlled testing environment.
- When testing untrusted or malicious code safely.
- When replicating a security environment on different systems.

**How:**
- Install Docker from: https://www.docker.com/products/docker-desktop
- Pull a Docker image:
  ```
  docker pull kalilinux/kali-rolling
  ```

- Run a container:
```
docker run -it kalilinux/kali-rolling /bin/bash
```
- Stop and remove the container when done:
```
docker ps
docker stop <container_id>
docker rm <container_id>
```

## 📌 Conclusion
Docker makes it easier for cybersecurity learners and professionals to:

Experiment safely

Run security tools

Create temporary lab environments

Analyze malware and vulnerabilities

---

Today We learnt what **NMap** is and it's different type of Commands and we also learnt about **Docker** and it's important in Cybersecurity. Do some research for extra useful insights and let's move to Our Day-08 (https://github.com/AnisurRahman-46/Cybersecurity-Learning/tree/main/Day-08)
