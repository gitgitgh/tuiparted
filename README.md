# TUIParted

🌐 **[English](README.md)** | **[Русский](README.ru.md)**

<p align="center">
  <b>Console Partition Manager</b><br>
  I tried to make a terminal disk partition manager with GParted-like functionality
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-linux-lightgrey.svg" alt="Linux">
  <img src="https://img.shields.io/badge/version-0.1.0b-orange.svg" alt="Version">
  <img src="https://img.shields.io/badge/license-MIT-green.svg" alt="MIT License">
</p>

---

## 📖 Description

**TUIParted** is a console-based partition manager that provides GParted-like functionality in a terminal interface. It offers an intuitive TUI (Text User Interface) for managing disk partitions.

### ✨ Features

- **📊 Visual Partition Bar** — Color-coded visualization of disk layout
- **💾 Multiple Filesystems** — Support for ext2/3/4, btrfs, xfs, f2fs, ntfs, fat32, exfat, swap
- **✅ Safe Operations Queue** — Preview changes before applying
- **🔧 Full Partition Management** — Create, delete, resize, move, copy partitions
- **🔍 Filesystem Tools** — Check (fsck), mount/unmount, automount configuration
- **🆘 Data Rescue** — Attempt to recover data from damaged partitions
- **🌍 Multi-language** — English, Russian. You can also add your own languages.
- **⌨️ Keyboard-driven** — Fast navigation with hotkeys
- **📁 Extended/Logical partitions** — Proper MBR hierarchy display

---

## 🚀 Usage

### Requirements

- Linux operating system
- Root privileges (for partition operations)
- Required packages: `parted`, `e2fsprogs`, `btrfs-progs`, `xfsprogs`, `rsync`

### Running

```bash
# Make executable (first time only)
chmod +x tuiparted

# Run with root privileges
sudo ./tuiparted
```

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `q` | Quit |
| `r` | Refresh disk data |
| `n` | Create new partition |
| `d` | Delete partition |
| `f` | Format partition |
| `s` | Resize partition |
| `t` | Create partition table |
| `c` | Check filesystem (fsck) |
| `i` | Show partition info |
| `l` | Select language |
| `Ctrl+A` | Apply pending operations |
| `Ctrl+Z` | Undo last operation |
| `←/→` | Navigate partitions |
| `Enter` | Open action menu |

---

## 🌍 Adding Languages

To add a new language:

1. Create `locales/` folder next to the binary
2. Create a JSON file (e.g., `fr.json`) — copy structure from existing translation
3. Restart the application

---

## 🔧 Supported Filesystems

| Filesystem | Create | Format | Resize | Check |
|------------|--------|--------|--------|-------|
| ext2/3/4 | ✅ | ✅ | ✅ | ✅ |
| btrfs | ✅ | ✅ | ✅ | ✅ |
| xfs | ✅ | ✅ | ✅ | ✅ |
| f2fs | ✅ | ✅ | ❌ | ✅ |
| ntfs | ✅ | ✅ | ✅ | ✅ |
| fat32/vfat | ✅ | ✅ | ✅ | ✅ |
| exfat | ✅ | ✅ | ❌ | ✅ |
| swap | ✅ | ✅ | ❌ | ❌ |

---

## ⚠️ Warning

**TUIParted performs low-level disk operations that can result in data loss.** Always:

- ✅ Back up important data before modifying partitions
- ✅ Review pending operations carefully before applying
- ✅ Ensure the target partition is not mounted

---

## ⚖️ Disclaimer

**USE AT YOUR OWN RISK.**

This software is provided "as is", without warranty of any kind, express or implied. The author is not responsible for any damages, data loss, or system failures arising from the use of this software.

By using TUIParted, you understand and acknowledge that:

1. **You are solely responsible** for any actions performed with this tool
2. **You have adequate backups** of all important data
3. **Partition operations are inherently dangerous** and can render your system inoperable
4. **The author assumes no responsibility** for any consequences of using this software

**Always test on systems without important data.**

---

## 💰 Support the Project

If you find this project useful, you can support development:

**USDT (TRC20):** `TEKrG4B6UW6iAHFS9GdkUzYye7iGCRMc6K`

---

## 📜 License

MIT License

---

## 👨‍💻 Author

**karamultuk**
