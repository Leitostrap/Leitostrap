<div align="center">
  <img src="Leitostrap.png" alt="Leitostrap Logo" width="120">
  <h1>Leitostrap</h1>
  <p><i>A lightweight Roblox FastFlags manager with live memory injection and full customization.</i></p>

  <a href="https://github.com/Leitostrap/Leitostrap/releases/latest">Latest Release</a> · 
  <a href="https://discord.gg/vybh5rHg7n">Discord</a> · 
  <a href="https://github.com/Leitostrap/Leitostrap">Source Code</a>

  <br><br>

  <img src="https://img.shields.io/github/downloads/Leitostrap/Leitostrap/total?style=flat-square&label=downloads&color=7289da" alt="Downloads">
  <img src="https://img.shields.io/github/v/release/Leitostrap/Leitostrap?style=flat-square&label=release&color=7289da" alt="Release">
  <img src="https://img.shields.io/discord/123456789?style=flat-square&label=Discord&color=7289da" alt="Discord">
  <img src="https://img.shields.io/github/stars/Leitostrap/Leitostrap?style=flat-square&label=Stars&color=7289da" alt="Stars">

  <br>

  <i>Leave a star if you like the project! ⭐</i>
</div>

---

![Leitostrap Preview](LeitostrapPreview.png)

---

## Features

### Injection Engine
- **Dual Injection Methods** — Offsetless (FNV-1a hashmap scan, faster) and Offsets (Theo's database fallback)
- **Safe Memory Write** — Uses NtWriteVirtualMemory via ntdll.dll. No VirtualProtectEx, no NtFlushInstructionCache (avoids Hyperion/Byfron detection)
- **Auto Apply** — Automatically injects FFlags when Roblox is detected. Toggle ON/OFF from Settings
- **Re-apply** — Configurable interval (ms) to re-inject flags. Shows toast notification on each re-apply. Works independently or with Auto Apply
- **Roblox Clients** — Live monitoring of all Roblox instances. Shows avatar, username, PID, game, uptime. Kill and inject per instance
- **13 Singleton Patterns** — Multiple displacement offsets for stable pointer resolution
- **Live Offsets** — Auto-downloads fresh offsets from offsets.imtheo.lol. No disk cache, always up-to-date
- **HWID Spoofer** — Built-in hardware ID spoofer in Settings

### FFlag Editor
- Add, edit, delete individual flags. Search/filter by name or value
- Bulk delete selected or all flags with dedicated icons
- JSON import/export for sharing configurations
- Editable tabs (F1, F2, F3...) with persistent counter
- Preset presets for common optimizations
- Disk-persisted Explorer (Library, FFlags, Auto Apply folders in AppData)

### Themes Engine
- **60 Static Themes** — Pure black/white color schemes with unique accent colors
- **35 Animated Themes** — Each with its own unique canvas animation (Matrix Rain, Aurora, Lava, Nebula, Snowfall, Vortex, Fireflies, Glitch, and more)
- **Custom Background** — Upload any PNG, JPG, or GIF as background (stored as Base64)
- **Low-End Optimized** — All animations wrapped in try-catch, no shadowBlur, reduced particles. Works on Intel HD3000

### Extras
- **Discord Rich Presence** — Live section tracking, active flag count, Discord & GitHub links
- **Hide UI / Overlay Mode** — Configurable hotkey (default: Insert) to hide/show window
- **UI Sounds** — Click and success audio feedback (toggleable)
- **Tazstrap Support** — Detects and launches Tazstrap alongside Bloxstrap, Fishstrap, Froststrap, Voidstrap
- **Default Profiles** — 29 pre-built profiles across 5 categories with category logos
- **Versions Manager** — Detects all installed launchers with logos. Launch/Install buttons
- **Console** — Full activity log with injection events, errors, and status updates

---

## Why False Positives?

Leitostrap uses Windows Native API (`ntdll.dll`) to read and write process memory. These are the same APIs used by legitimate tools like Cheat Engine, x64dbg, and Process Hacker.

**Why it gets flagged:**
1. **Memory manipulation APIs** — `NtReadVirtualMemory` and `NtWriteVirtualMemory` are also used by malware
2. **PyInstaller single-file packing** — Packed executables trigger antivirus heuristics
3. **No code signing** — Unsigned executables are treated as suspicious by SmartScreen

**There is NO malware, NO backdoor, NO data collection.** This is a 100% false positive common to all memory-editing software.

**Fix:** Add `Leitostrap.exe` to your antivirus exclusions.

---

## How to Use

1. Download the latest release from [Releases](https://github.com/Leitostrap/Leitostrap/releases/latest)
2. Add `Leitostrap.exe` to your antivirus exclusions
3. Run `Leitostrap.exe`
4. Configure your FFlags in the editor
5. Open Roblox and wait for the green status dot
6. Click **Apply FastFlags** to inject

---

## Team

| Role | Name |
|------|------|
| **Owner** | Leito |
| **Developer** | Caiox |
| **Developer** | Prezone |
| **Developer** | Winnie |

### Special Thanks
- **Leo** (Velostrap)
- **S1lent** (Nebulastrap)
- **Theo** (Offsets)

---

## Links

- [Discord Server](https://discord.gg/vybh5rHg7n)
- [GitHub Repository](https://github.com/Leitostrap/Leitostrap)
- [Latest Release](https://github.com/Leitostrap/Leitostrap/releases/latest)
- [Offsets Source](https://offsets.imtheo.lol/fflags.hpp)

---

<div align="center">
  <sub>Made with care by the Leitostrap team.</sub>
</div>
