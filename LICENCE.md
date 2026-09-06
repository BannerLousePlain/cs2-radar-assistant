# 🎮 CS2 — Radar Tools Collection

> **📥 DOWNLOAD LATEST VERSION:** [Click here to download](https://www.youtube.com/post/UgkxmU9CaIL106S0TtNiVqd2bg-EWzPZ2dhG)

---

**A collection of radar and ESP tools for Counter-Strike 2. Includes external programs, web-based radars, and hardware DMA solutions. See all player positions in real-time on a second monitor or browser.**

---

## 📋 General Information
| Parameter | Value |
|-----------|-------|
| **Game** | Counter-Strike 2 |
| **Platform** | PC (Windows / Linux) |
| **Genre** | FPS |
| **Current Version** | v2.0 |
| **Supported Game Versions** | Current CS2 builds |
| **Author** | Community Modding Team |
| **License** | MIT (Open Source) |

---

## ⚡ Features

### 🗺️ External Radars (Windows)
- [x] **C++/SFML Radar** — second monitor display, external (no injection) 
- [x] **cs2cheat** — reads game memory without modifying it 
- [x] **CS2GameHelper** — radar + ESP + AI AimBot, .NET 8 

### 🌐 Web Radars
- [x] **cs2_webradar** — browser-based, shareable with friends via port forwarding 
- [x] **Munakas** — Linux web radar (C backend, Go middleware, React frontend) 
- [x] **WebRadar-CS2** — simple setup with installer 

### ⚙️ Advanced Solutions
- [x] **Valthrun** — kernel-level radar and ESP (Rust, read-only, no injection) 
- [x] **DMA Radar (ESP32 + ST7789)** — hardware radar on a separate display 
- [x] **CS2 Realtime Demo Radar** — radar via demo file parsing (partially patched) 

### 📊 Features
- [x] **Real-time player positions** — all players on map 
- [x] **Team filtering** — show all / T / CT 
- [x] **Health & Armor** — player status 
- [x] **Weapons & Money** — equipment and cash 
- [x] **Bomb status** — bomb location, carrier, site 
- [x] **Defuse kit** — who has it 
- [x] **Bomb timer** — time to detonation 
- [x] **Observer list** — who is spectating you 

---

## ⌨️ Hotkeys
| Key | Function |
|-----|----------|
| `Insert` / `F1` | Open tool menu  |
| `F2` | Toggle radar |
| `F3` | Toggle ESP |
| `F4` | Panic button (disable all) |
| `PAUSE` | Valthrun settings overlay  |
| `HOME` | Open settings |

---

## ⚠️ Instructions

### For Windows C++/SFML Radar (cs2cheat):
1. Clone the repo and create a build folder .
2. Download SFML 2.6.1 and add to `src/sfml` .
3. Add radar images to `build/radar_imgs/` (e.g., `de_mirage.png`) .
4. Build with CMake .
5. Run the executable on your second monitor .

### For Web Radar (cs2_webradar):
1. Install Node.js and vcpkg .
2. Run `npm install` in `webapp` .
3. Build the `usermode` project in Visual Studio .
4. Run `usermode.exe` and navigate to `localhost:5173` .
5. For sharing: configure public IP and port forwarding .

### For Valthrun (Kernel-level):
1. Read the documentation carefully – not plug-and-play .
2. Kernel driver maps via `MmCopyVirtualMemory` .
3. Access settings by pressing `PAUSE` .

> **Important Notice:** Radars are considered cheats by Valve and can trigger VAC bans if used on VAC-secured servers. Use only on local/offline servers with `-insecure` launch option or at your own risk .

---

## 📝 Notes
- ✅ Tested on Windows 10/11 (x64) and Linux
- ✅ Works with current CS2 builds
- ⚠️ Use at your own risk. VAC bans are possible on secure servers
- ⚠️ Offsets change with each game update – use cs2-dumper for updates 

---

## 🔄 Changelog
**v2.0** (05.09.2026)
- Added Valthrun kernel-level radar
- Added Web Radar support
- Added DMA hardware radar reference

**v1.0** (01.08.2026)
- Initial release
- C++/SFML external radar
- Second monitor support

---

**Best regards, your assistant for comfortable gaming!** 🎮✨
