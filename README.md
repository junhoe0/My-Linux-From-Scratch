# <p align="center"> Linux From Scratch </p>
<p align="center">An independent implementation of the Linux From Scratch (Systemd Edition) book entirely from the source code. This repository serves as documented proof of compilation, configuration and successful system boot.</p>
  
---  

## 🚀 Project Overview
|**Parameter**|**Specification**|
|:---|:---|
| Book Version | Linux From Scratch (Systemd Edition) v13.0
| Host OS | Linux Mint
| LFS Kernel Version | Linux 6.18.10
| Target Architecture | x86_64
| Networking Stack | NetworkManager (instead of systemd-networkd)
| Build Method | Fully Manual Entry
| Host Machine | Thinkpad T490s

---  

## 🛠️ Proof Of Implementation
To verify that the system is bootable and completely operational, I have included some artifacts in this repository:
1. Kernel Configuration
2. Systemd Boot Logs
3. System Control Status

---

## 📦 Repository Structure
```
├── README.md  
├── kernel.config  
└── logs/  
    ├── boot.log  
    └── systemctl-status.txt
```

---

## 🎓 What I've Learned
* Useful yet simple CLI tools (e.g cp, mv, find, mkdir, mount)
* How to manually extract, compile and install packages directly from source code using 'autotools' (./configure, make, make install)
* Configuring the Linux Kernel to meet package requirements
* Creating a temporary cross-compiler toolchain isolated from the host environment
* Resolving missing dependencies without a package manager

---  

## ⚠️ Challenges Faced
 * Debugging Boot Problems - On first boot, my laptop displayed unable to find vmlinuz. After trying to fix it, I accidentally binding /dev to wrong file and had to reinstall Linux Mint  
 * Downloading, compiling and installing NetworkManager - I had to install up to 13 different packages manually, each package branching out with more dependencies, making sure non of the commands have typos  
