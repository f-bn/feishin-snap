<p align="center">
  <img src="snap/gui/feishin.png" alt="Feishin" width="128" />
</p>

---

## 📋 Overview

This repository contains an unofficial snap package recipe for [Feishin](https://github.com/jeffvli/feishin).

## 🚀 Quick Start

### 📦 Setup Snapcraft (with Multipass backend)

1. Install Snapcraft and Multipass:
   ```bash
   task setup
   ```

2. Verify both are installed:
   ```bash
   snapcraft --version
   multipass --version
   ```

### 🛠️ Build

1. Clone the repository:

   ```bash
   git clone https://github.com/f-bn/feishin-snap.git
   cd feishin-snap
   ```

2. Build the snapcraft package:

   ```bash
   task build
   ```

3. Install the locally built snap:

   ```bash
   task install
   ```

## ✅ Checklist

- [x] Disable auto-updates
- [x] Media control via MPRIS
- [x] Password storage to system keyring (validated against GNOME keyring)
- [x] Remote Control server
- [ ] MPV backend
- [ ] ~~Discord Rich Presence (if possible, especially with Discord snap)~~
- [ ] Publish to Snap store