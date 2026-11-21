<p align="center">
  <img src="docs/logo.png" alt="TH Suite" width="220">
</p>

<h1 align="center">TH Suite</h1>

<p align="center">
  All-in-one Windows optimization: tweaks, RAM, cleanup, uninstaller, hardware, gaming network, security and repairs.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-0078D6?logo=windows" alt="Windows">
  <img src="https://img.shields.io/badge/.NET-8-512BD4?logo=dotnet" alt=".NET 8">
  <img src="https://img.shields.io/badge/license-MIT-green" alt="MIT License">
</p>

<p align="center"><a href="LEIAME.md">🇧🇷 Leia em português</a></p>

---

TH Suite combines **TH Reduct**, **TH Cleaner**, **TH Control** and **TH Guard** with a **Windows optimizer** and a **repair center**. Every option explains what it does, when it helps and when not to use it. The interface is in Portuguese.

## ✨ Features

### 🏠 Home
- **PC health score** (memory, disk, pending tweaks, security) with a shortcut to fix each issue
- One-click **quick optimization**: restore point, RAM, junk files, safe tweaks and DNS
- Live CPU, RAM, disk and antivirus status, plus system information

### ⚡ Optimizer (80+ tweaks)
- **Performance**, **Gaming**, **Power**, **Graphics card** (HAGS, MPO, TDR, NVIDIA telemetry, AMD ULPS), **Network**, **Privacy**, **Windows 11**, **Services** and **Windows Update**
- Each tweak shows a **risk level**, a full explanation, laptop and restart notices
- Nothing changes until you click **Apply**; original values are saved so **every tweak can be undone**
- Automatic **restore point** before applying
- **Debloat**: remove preinstalled apps without touching essential ones

### 🧠 RAM
- Working set, system cache, modified and standby list cleanup; automatic cleanup and alerts
- **Game mode** with priority, power plan and pausing heavy apps; in-game widget; global hotkey

### 🧹 Cleanup and uninstaller
- Windows, browser and app caches, large files, full uninstaller with **leftover removal** and registry backup, Store apps

### 🌡️ Hardware and network
- Temperatures, load, clocks, power, disks and fans (LibreHardwareMonitor)
- Fan/power profiles; **gaming network**: DNS benchmark, Nagle, throttling and QoS

### 🛡️ Security
- Smart scan + Microsoft Defender + VirusTotal (optional)
- **Hidden miner detection**, masquerading processes, double extensions, suspicious startup entries, reversible quarantine

### 🔧 Repairs and tools
- 31 explained one-click repairs (network, Wi-Fi, Bluetooth, audio, camera, printer, DISM + SFC, missing DLLs, Windows Update, Start menu, icons, PIN, Store, Xbox, Defender, high CPU/RAM/disk...) with live output
- Quick tools: restore point, restart Explorer, reboot to BIOS or recovery, Windows shortcuts

### 🎨 Customization
- Dark, black and light themes, accent colors and **logo colors**; tray icon with RAM %; start with Windows

## 📥 Download

Get the latest version from [**Releases**](https://github.com/Thiagosystems/THSuite/releases).

> Nothing to install: the .exe already includes .NET. Works on Windows 10/11 64-bit and requires **administrator** rights.

## 🛠️ Build

Requirement: [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)

```bat
git clone https://github.com/Thiagosystems/THSuite.git
cd THSuite
build.bat
```

The executable is created at `publish\THSuite.exe`.

## ⚠️ Notes

- **Advanced** tweaks reduce security or disable features; read the warning first.
- Security heuristics may produce false positives.

## 📄 License

Released under the MIT License. See [LICENSE](LICENSE). Third-party libraries in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
