# RTL8188FU Monitor Mode – KernelSU / Magisk Modules

[![status](https://img.shields.io/badge/status-stable-brightgreen)](https://github.com/nsluisr/rtl8188fu-driver-samsung-a05)  
[![license](https://img.shields.io/badge/license-GPL--2.0-blue)](https://github.com/nsluisr/rtl8188fu-driver-samsung-a05/blob/main/LICENSE)

**Repository:** `rtl8188fu-driver-samsung-a05`  
USB WiFi driver for **RTL8188FU** chipsets with full **monitor mode support**, packaged as a **KernelSU** or **Magisk** module.  
**Patched and optimized for Samsung Galaxy A05M (Android ARM64)** by sluisr.

---

## 📦 Features

- ✅ Monitor Mode enabled (verified via `iw list`)  
- ✅ Support for Realtek **RTL8188FU** chipsets  
- ✅ Flashable `.zip` modules (KernelSU or Magisk compatible)  
- ⚙️ Kernel compatibility: **4.4 to 5.15**  
- 🔧 Includes critical fixes for `cfg80211` and USB suspend  
- 📱 **Tested and optimized for Samsung A05M**

---

## 📂 Available Modules

| Version       | Mode          | Platform        | File Name                        |
|---------------|---------------|-----------------|---------------------------------|
| `4.0 Monitor` | Monitor Mode  | KernelSU/Magisk | `rtl8188fu_module_monitor.zip`  |
| `3.0 Stable`  | Normal Mode   | KernelSU/Magisk | `rtl8188fu_module_stable.zip`   |

---

## 🔧 Installation

### ✅ KernelSU

1. Copy the `.zip` file to your internal storage.  
2. Open the **KernelSU Manager** app.  
3. Go to **Modules → + → From Storage** and select the module.  
4. Reboot your device.

### ✅ Magisk

1. Open **Magisk Manager**.  
2. Go to **Modules → Install from storage**.  
3. Choose the `.zip` module file.  
4. Reboot your device.

---

## 📡 Enabling Monitor Mode

```bash
# Check monitor mode support
iw list

# Kill interfering processes
sudo airmon-ng check kill

# Start monitor mode on wlan1 (or your interface)
sudo airmon-ng start wlan1
```

---

---

## 🙏 Credits

This project builds upon work from the following repositories:

### 🔧 Primary Development Repositories
- [Foxy6670/rtl8188fu-mon](https://github.com/Foxy6670/rtl8188fu-mon) – Monitor mode implementation
- [kelebek333/rtl8188fu](https://github.com/kelebek333/rtl8188fu) – Base driver without monitor mode

### 🧬 Original Source
- [ulli-kroll/rtl8188fu](https://github.com/ulli-kroll/rtl8188fu) – Original Realtek driver source

> Special thanks to all contributors and maintainers of these projects.

---
