# Syscall

[![AUR](https://img.shields.io/aur/version/syscall?logo=arch-linux&label=AUR)](https://aur.archlinux.org/packages/syscall)
[![License](https://img.shields.io/github/license/YOURNAME/syscall)]()
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
