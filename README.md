# <p align="center"> Linux From Scratch </p>
<p align="center">An independent implementation of the Linux From Scratch (Systemd Edition) book entirely from the source code. This repository serves as documented proof of compilation, configuration and successful system boot.</p>
  
---  

## 🚀 Project Overview
1. Book Version : Linux From Scratch (Systemd Edition) 
2. Host OS : Linux Mint
3. LFS Kernel Version : Linux 6.18.10
4. Target Architecture : x86_64
5. Networking Stack : NetworkManager (instead of systemd-networkd)
6. Build Method : Fully Manual Entry
7. Host Machine : Thinkpad T490s

---  

## 🛠️ Proof Of Implementation
To verify that the system is bootable and completely operational, I have included some artifacts in this repository:
1. Kernel Configuration
2. Systemd Boot Logs
3. System Control Status
4. Configuration Directory

---  

## 🎓 What I've Learned
1. Useful yet simple CLI tools (e.g cp, mv, find, mkdir, mount)
2. How to manually extract, compile and install packages directly from source code using 'autotools' (./configure, make, make install)
3. How to install packages from the internet in CLI
4. Cross-compiling temporary tools to build the system

---  

## ⚠️ Challenges Faced
 • Debugging Boot Problems - On first boot, my laptop displayed unable to find vmlinuz. After trying to fix it, I accidentally binding /dev to wrong file and had to reinstall Linux Mint
 • Downloading, compiling and installing NetworkManager - I had to install up to 13 different packages manually, each package branching out with more dependencies, making sure non of the commands have typos
