Here's the updated README with the new Downloads section added right after the Available Modules table:

# RTL8188FU Monitor Mode – KernelSU / Magisk Modules

[![status](https://img.shields.io/badge/status-stable-brightgreen)](https://github.com/nsluisr/rtl8188fu-driver-samsung-a05)  
[![license](https://img.shields.io/badge/license-GPL--2.0-blue)](https://github.com/nsluisr/rtl8188fu-driver-samsung-a05/blob/main/LICENSE)

**Repository:** `rtl8188fu-driver-samsung-a05`  
USB WiFi driver for **RTL8188FU** chipsets with full **monitor mode support**, packaged as **KernelSU** or **Magisk** modules.  
**Patched and optimized for Samsung Galaxy A05M (Android ARM64)** by sluisr.

---

## 📦 Features

- ✅ Monitor Mode enabled (verified via `iw list`)  
- ✅ Support for Realtek **RTL8188FU** chipsets  
- ✅ Flashable `.zip` modules (KernelSU/Magisk compatible)  
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

## 📥 Downloads

Get the latest modules from the [Releases](https://github.com/nsluisr/rtl8188fu-driver-samsung-a05/releases) page:

- 💣 [rtl8188fu_module_monitor.zip](https://github.com/nsluisr/rtl8188fu-driver-samsung-a05/releases/latest) – Monitor Mode (v4.0)
- 🧱 [rtl8188fu_module_stable.zip](https://github.com/nsluisr/rtl8188fu-driver-samsung-a05/releases/latest) – Stable Mode (v3.0)

> Make sure to pick the right file for your setup (KernelSU or Magisk).

---

## 🔧 Installation

### ✅ KernelSU

1. Copy the `.zip` file to your device's storage  
2. Open **KernelSU Manager**  
3. Navigate to **Modules → + → From Storage** and select the module  
4. Reboot your device

### ✅ Magisk

1. Open **Magisk Manager**  
2. Go to **Modules → Install from storage**  
3. Select the module `.zip` file  
4. Reboot your device

---

## 📡 Enabling Monitor Mode

```bash
# Verify monitor mode support
iw list

# Terminate interfering services
sudo airmon-ng check kill

# Enable monitor mode (replace wlan1 with your interface)
sudo airmon-ng start wlan1
```

---

## 🙏 Credits & Resources

### Development Repositories
- **[Foxy6670/rtl8188fu-mon](https://github.com/Foxy6670/rtl8188fu-mon)**  
- **[kelebek333/rtl8188fu](https://github.com/kelebek333/rtl8188fu)**  
- **[ulli-kroll/rtl8188fu](https://github.com/ulli-kroll/rtl8188fu)**  

---

## 🚀 Show Your Support
⭐ **Star the GitHub Repository**  
🐛 **Report issues on GitHub**  
