# 🛠️ Tools Installation Checklist (with Version Checks)

This document tracks the progress of my SFAL/VSD tool installation 

---

## ✅ Task 1 – GitHub Setup
- [ ] **Create GitHub Repository**
  - Repo Name: `vsd-tool-installation` 
- [ ] **Add Summary of Previous Video**
  - Added a `README.md` or markdown file summarizing Day 0 video  

---

## ✅ Task 2 – Tool Installation

> **System Requirements**
> - Ubuntu 20.04+  
> - 6 GB RAM  
> - 50 GB HDD  
> - 4 vCPUs  

---

1️⃣ Yosys
**Install:**
```bash
sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make
sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install

