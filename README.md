Leitostrap - Roblox FastFlags Manager & Injector

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

A lightweight, modern Roblox FastFlags manager with live memory
injection, dual injection methods, and full UI customization.
Built with Python + PyWebView. All assets embedded in source.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

FEATURES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

INJECTION
  • Dual injection: Offsetless (FNV-1a) + Offsets (Theo fallback)
  • Safe write: NtWriteVirtualMemory, no VirtualProtectEx
  • Auto Apply: injects when Roblox detected
  • Re-apply: configurable interval re-injection
  • 13 singleton patterns, live offsets from imtheo.lol
  • HWID Spoofer built-in

EDITOR
  • Add, edit, delete, search FFlags
  • Bulk delete selected / all
  • JSON import/export
  • Editable tabs with persistent counter
  • Preset presets for common optimizations
  • Disk-persisted Explorer (Library, FFlags, Auto Apply)

MONITORING
  • Roblox Clients: avatar, username, PID, game, uptime
  • Kill and inject per instance
  • Live process detection with green/red status

UI & THEMES
  • 60 static themes (pure black/white, no purple)
  • 35 animated themes (each with unique canvas animation)
  • Custom background import (PNG/JPG/GIF, Base64 stored)
  • Low-end GPU optimized (no shadowBlur, try-catch)
  • Neon gradient title text, frameless window
  • Splash screen with logo split animation

EXTRAS
  • Discord Rich Presence with section tracking
  • Hide UI / Overlay mode (configurable hotkey)
  • UI sounds (toggleable)
  • Tazstrap support (alongside 4 other launchers)
  • 29 default profiles in 5 categories with logos
  • Versions manager with launcher detection
  • Console activity log

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

TEAM
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  Owner:       Leito
  Developers:  Caiox, Prezone, Winnie

  Special Thanks:
  • Leo (Velostrap)
  • S1lent (Nebulastrap)
  • Theo (Offsets)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

ANTIVIRUS FALSE POSITIVES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Leitostrap uses Windows Native API (ntdll.dll) to read and
write process memory. This is the same approach used by
legitimate tools like Cheat Engine, x64dbg, and Process Hacker.

False positives occur because:

  1. Memory manipulation APIs (NtReadVirtualMemory,
     NtWriteVirtualMemory) are also used by malware

  2. PyInstaller single-file compilation triggers
     heuristic detection in packed executables

  3. No code signing certificate means SmartScreen
     flags the unsigned executable

There is NO malware, NO backdoor, NO data collection.
This is a FALSE POSITIVE common to all memory-editing software.

Fix: Add Leitostrap.exe to your antivirus exclusions.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

TECHNICAL DETAILS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  • Language:    Python 3.12
  • UI:          PyWebView 6.2.1 (HTML/CSS/JS)
  • Injection:   ntdll.dll (NtReadVirtualMemory, NtWriteVirtualMemory)
  • Build:       PyInstaller (--onefile --windowed)
  • AppData:     %APPDATA%/Leitostrap Injector/
  • Offsets:     https://offsets.imtheo.lol/fflags.hpp
  • Discord:     https://discord.gg/vybh5rHg7n

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
