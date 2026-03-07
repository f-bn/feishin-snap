# Feishin Snap

Unofficial snap package for [Feishin](https://github.com/jeffvli/feishin).

## Setup

### Setup Snapcraft (with Multipass backend)

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

## Build

Clone the repository:

```bash
git clone https://github.com/f-bn/feishin-snap.git
```

Build the snapcraft package:

```bash
snapcraft pack
```

> [!NOTE]
> Snapcraft will launch a Multipass VM, build the snap inside it, and output a `.snap` file in the current directory.

To install the locally built snap:

```bash
sudo snap install feishin_*.snap --dangerous
```

After installation, connect the required interface for secure password storage:

```bash
sudo snap connect feishin:password-manager-service
```

## Validation checklist

- [x] Disable auto-updates
- [x] Ensure media control via MPRIS
- [x] Password storage to system keyring (validated against GNOME keyring) 
- [ ] MPV backend
- [ ] Discord Rich Presence (if possible, especially with Discord snap)