# 🐧 Linux System & Network Administration Project

![Linux](https://img.shields.io/badge/OS-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Ubuntu](https://img.shields.io/badge/Distro-Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![VirtualBox](https://img.shields.io/badge/Virtualization-VirtualBox-183A61?style=for-the-badge&logo=virtualbox)
![Bash](https://img.shields.io/badge/Scripting-Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Apache](https://img.shields.io/badge/Web-Apache-D22128?style=for-the-badge&logo=apache)
![Security](https://img.shields.io/badge/Focus-Cybersecurity-0A0A0A?style=for-the-badge&logo=hackaday)

---

## 📌 Project Overview
This repository contains my complete implementation of a **Linux System and Network Administration** case study carried out as part of the **IE2012 – Systems and Network Programming** module.

The project focuses on configuring core Linux network services, implementing security mechanisms, automating system tasks, deploying servers, and performing **binary debugging and reverse engineering using GDB**.

This work demonstrates hands-on skills relevant to **Linux system administration, cybersecurity, and network engineering roles**.

---

## 🛠️ Technologies & Tools Used
- Ubuntu Linux (VirtualBox VM)
- Linux Command Line & Shell Scripting
- DHCP, DNS (BIND9), and NTP (NTPsec)
- OpenSSH Server
- iptables Firewall Rules
- Apache Web Server
- Postfix Email Server
- Cron Jobs & Log Management
- GDB Debugger
- Hexdump & Strings Analysis Tools
- C Programming (XOR Encryption / Decryption)

---

## 📂 Project Sections

### 1. Basics of Linux Environments
- VirtualBox installation and VM configuration
- Ubuntu Desktop installation
- Command-line navigation and file management
- System information commands
- User and group management

---

### 2. DHCP, DNS, and NTP Services

#### 🔸 DHCP (Dynamic Host Configuration Protocol)
- Installed and configured **isc-dhcp-server**
- Used dual network adapters (NAT + Internal Network)
- Created custom IP scope: `192.168.100.20 – 192.168.100.30`
- Assigned static IP to DHCP interface
- Verified DHCP leases from a client machine

#### 🔸 DNS (Domain Name System – BIND9)
- Installed and configured **BIND9**
- Created local forward lookup zones (e.g., `lab.local`)
- Enabled hostname → IP and IP → hostname resolution
- Integrated DNS with DHCP
- Configured Google DNS (`8.8.8.8`) as a forwarder
- Verified resolution using `dig` on server and client

#### 🔸 NTP (Network Time Protocol)
- Installed and configured **NTPsec**
- Synchronized system time using:
  - `time1.google.com`
  - `pool.ntp.org` (fallback)
- Verified synchronization using `ntpq -p`

---

### 3. Security and Server Configuration

#### 🔸 Shell Scripting & Automation
- Created a **log cleanup and archival script**
- Deleted logs older than 7 days
- Archived active logs into compressed backups
- Generated execution summaries
- Scheduled weekly execution using **cron**

#### 🔸 SSH (Secure Shell)
- Installed and configured OpenSSH
- Changed default SSH port to `2222`
- Forced IPv4 connections only
- Restricted SSH access to specific network interfaces
- Implemented **key-based authentication (Ed25519)**
- Verified secure client connections

#### 🔸 Firewall Rules (iptables)
- Cleared existing firewall rules
- Blocked access to:
  - Facebook
  - Instagram
  - Twitter
- Blocked HTTP traffic (port `80`)
- Allowed HTTPS traffic (port `443`)
- Verified rules using `iptables -L`

#### 🔸 Apache Web Server
- Installed and configured Apache2
- Created and hosted a custom HTML page
- Set correct file ownership and permissions
- Accessed the hosted page via a client browser

#### 🔸 Postfix Email Server
- Installed Postfix in **Internet Site mode**
- Configured hostname and default settings
- Tested internal mail delivery using **Mutt**
- Verified successful mail delivery through log analysis

---

### 4. Linux GDB – Debugging & File Analysis

#### 🔸 Binary Execution & Initial Analysis
- Executed an unknown ELF binary
- Observed creation of encrypted `data.txt`
- Analyzed files using:
  - `cat`
  - `file`
  - `hexdump`
  - `strings`

#### 🔸 GDB Debugging
- Inspected executable using **GDB**
- Identified XOR-based encryption function
- Set breakpoints and disassembled functions
- Inspected registers and memory
- Extracted encryption key and plaintext source

#### 🔸 Decryption & Verification
- Wrote a custom **C program** to decrypt encrypted data
- Used extracted XOR key
- Successfully recovered original plaintext
- Confirmed symmetric XOR encryption behavior

---

## 🔐 Key Skills Demonstrated
- Linux system administration
- Network service deployment (DHCP, DNS, NTP)
- Firewall and access control management
- Secure remote access (SSH hardening)
- Shell scripting & automation
- Web and email server configuration
- Reverse engineering fundamentals
- Debugging binaries with GDB
- Encryption and decryption logic analysis
- File system and log analysis

---

## 📚 Academic Context
- **Institute:** Sri Lanka Institute of Information Technology (SLIIT)
- **Module:** IE2012 – Systems and Network Programming
- **Project Type:** Linux Administration Case Study

---

⭐ *If you find this project useful, feel free to star the repository!*  
