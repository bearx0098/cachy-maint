# CachyOS Maintenance Utility

A professional system maintenance and update tool designed for CachyOS and Arch Linux. This utility automates the cleanup of package caches, removal of orphans, and performs a comprehensive system update using `topgrade`.

## Features
- **One-Command Maintenance:** Clean your system and update everything in one go.
- **Cache Optimization:** Clears out old `pacman` and `paru` download caches to save disk space.
- **Orphan Cleanup:** Automatically identifies and removes unneeded dependencies.
- **Meta-Updates:** Leverages `topgrade` to update system packages, AUR, and firmware.
- **Error Tracking:** Automatically generates logs in `~/.local/share/cachy-maint/logs` if a process fails.

---

## Installation

### Method 1: Automatic Installation (Recommended)
If you are using an AUR helper like `paru` (standard on CachyOS) or `yay`, you can install the utility directly once it is available on the AUR:
```bash
paru -S cachy-maint-utility
```
### Method 2: Semi-Manual (Git Clone)
Use this method if you want to stay up to date with the latest source code from GitHub:
1. **Clone the repository:**
```bash
git clone [https://github.com/bearx0098/cachy-maint-utility.git](https://github.com/bearx0098/cachy-maint-utility.git)
```
2. **Enter the directory:**
```bash
cd cachy-maint-utility
```
3. **Build and Install:**
```bash
makepkg -sif
```
### Method 3: Manual (ZIP / Release Download)
Use this method if you downloaded the source code as a .zip or .tar.gz from the GitHub Releases page:
1. **Extract the archive** and open a terminal inside the extracted folder.
2. **Install build dependencies** (if not already present):
```bash
sudo pacman -S --needed base-devel
```
3. **Build and Install:**
```bash
makepkg -sif
```
## Usage
### From the Launcher
You can find the utility in your application menu (KDE, GNOME, etc.) under the name "System Maintenance".
### From the Terminal
Simply type the following command:
```bash
cachy-maint
```
## Dependencies
This utility relies on the following packages (installed automatically if using `makepkg` or `paru`):

* **bash**: Script execution environment.
* **pacman**: Core system package management.
* **pacman-contrib**: Required for the `paccache` utility.
* **paru**: Used for AUR maintenance and orphan detection.
* **topgrade**: Orchestrates the multi-layered system updates.
* **perl**: Cleans ANSI color codes from generated error logs.
## License
Copyright (C) 2026 bearx0098 <bearx0098@gmail.com>

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.html) for more details.
