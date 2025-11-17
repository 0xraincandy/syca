# Syscall

[![AUR](https://img.shields.io/aur/version/syscall?logo=arch-linux&label=AUR)](https://aur.archlinux.org/packages/syscall)
[![License](https://img.shields.io/badge/license-GPLv3-brightgreen)]()
[![Language](https://img.shields.io/badge/language-Python%20%2B%20C-blue)]()

A minimal **sudo-like privilege elevation tool for Linux**, written in **Python + C**  
with **PAM authentication** and **system-wide secure password caching**.

Syscall acts as a clean, lightweight alternative to sudo/doas while keeping strict  
security boundaries. Authentication is performed via PAM, and a secure C setuid helper  
executes privileged commands safely.

---

## ✨ Features

- 🔐 **PAM-based password authentication**  
- 🕒 **System-wide privilege cache** (shared across all terminals)  
- ⚙️ **Execute commands as root:**  
  ```bash
  syscall <command>

## 🚀 Usage

Run any command as root via syscall:

```bash
# Update system packages
syscall pacman -Syu

# Restart a system service
syscall systemctl restart NetworkManager

# Edit a root-owned file
syscall nano /etc/hosts


---

### **Installation from AUR**

```markdown
## 📦 Installation

### From the AUR

Install directly using an AUR helper like yay or paru:

```bash
yay -S syscall


---

### **Manual Installation**

```markdown
### Manual Install

Clone the repository and build the package manually:

```bash
git clone https://github.com/YOURNAME/syscall.git
cd syscall
makepkg -si

