<p align="center">
  <img src="snap/gui/feishin.png" alt="Feishin" width="128" />
</p>

---

## 📋 Overview

This repository contains an unofficial snap package recipe for [Feishin](https://github.com/jeffvli/feishin).

## 🚀 Quick Start

### 📦 Setup Snapcraft (with Multipass backend)

1. Install Snapcraft:
   ```bash
   sudo snap install snapcraft --classic
   ```

2. Install Multipass:
   ```bash
   sudo snap install multipass
   ```

3. Verify both are installed:
   ```bash
   snapcraft --version
   multipass --version
   ```

### 🛠️ Build

1. Clone the repository:

   ```bash
   git clone https://github.com/f-bn/feishin-snap.git
   ```

2. Build the snapcraft package:

   ```bash
   snapcraft pack
   ```

3. Install the locally built snap:

   ```bash
   sudo snap install feishin_*.snap --dangerous
   ```

4. After installation, connect the required interface for secure password storage:

   ```bash
   sudo snap connect feishin:password-manager-service
   ```

## ✅ Checklist

- [x] Disable auto-updates
- [x] Media control via MPRIS
- [x] Password storage to system keyring (validated against GNOME keyring)
- [ ] Remote Control server
- [ ] MPV backend
- [ ] Discord Rich Presence (if possible, especially with Discord snap)
- [ ] Publish to Snap store