<div align="center">

# 🎮 Game Specific Patches & DLL Wrappers  

**created and maintained by**

[![Chip-Biscuit Website](https://img.shields.io/badge/Chip--Biscuit-Website-blue?style=for-the-badge)](https://chip-biscuit.github.io/)

Reverse Engineering • Programming • Patching • Game Preservation • DLL Creation 

</div>

---

# Star Wars: Episode I – Battle for Naboo  
### 64-bit Installer With Modern Game Fixes

A complete, preservation-grade 64-bit replacement installer for the **original 1999 PC release**, rebuilt from scratch for modern versions of Windows.

This is the **definitive way to install and play** *Star Wars: Episode I – Battle for Naboo* on modern hardware, with full widescreen support, DX9 translation, stability fixes (all optional), and resolution unlocking.

---

# Why This Installer Exists

The original retail PC release uses a **16-bit Windows installer**, which will not run on any 64-bit version of Windows.  
This makes the game effectively un-installable on modern systems.

To preserve the game, I fully rebuilt the installer into a native 64-bit modern version that:

- Works on all modern versions of Windows
- Requires the original retail PC disc
- Does **not** redistribute game files
- Recreates the full install logic
- Includes optional modern fixes and enhancements
- Repairs permissions so the game can write configs normally

---

# Installation

1. Download the installer from the **Releases** page:  
   **`Chips64bit_BattleForNabooInstaller.exe`**

2. Mount your original game disc.

3. When the installer launches, browse to the **root of the disc** (e.g. `D:\`).

4. Follow the on-screen instructions.

5. A desktop shortcut will be created. Launch and play.

---

# Requirements

### You must own the original English retail PC CD  
No game files are included or distributed. You must mount the disc before running the installer.

Common mount locations:
```
D:\
E:\
F:\
```

Browse to the disc on the installer’s first page.

---

# Features

## Modern Fix Pack (Optional)  Alternatively in the installer you can uncheck the option for the Fixes and install only the base game

---

### UCyborg’s Legacy D3D Resolution Hack
Unlocks modern GPU-reported resolutions including:
- 1080p
- 1440p
- Ultrawide
- Full native 4K
--- 

### ElishaCloud’s DXWrapper (D3D7 → D3D9)
Adds:
- Anti-aliasing
- Anisotropic filtering
- DX7 → DX9 translation
- Fix for the **thruster bug** on >60Hz monitors
  
---

### ThirteenAG’s Ultimate ASI Loader
Automatically loads all included `.asi` plugins located in `data_pc/plugins/`.

---

### Full Folder Permission Repair
The installer automatically:
- Removes read-only CD attributes  
- Fixes NTFS permissions  
- Allows editing INI files  
- Prevents write errors from wrappers or plugins
  
---

### AlphaYellow’s Widescreen & FOV Fix
Corrects the aspect ratio and field of view on all widescreen and ultrawide resolutions. Can be edited within (StarWarsEpisode1BattleForNabooFOVFix.ini):

```
Width=1920
Height=1080

```
### ChipResolution – Custom Resolution Support
Allows entering resolutions such as:
```
1920x1080

```
The installer writes these directly to the game’s registry key.

### ⚠️ Important – Resolution Values Must Match

The resolution in **ChipResolution.ini**  
(e.g. `Screen=1920x1080`)

must always match the resolution in  
**StarWarsEpisode1BattleForNabooFOVFix.ini**  
(e.g. `Width=1920` and `Height=1080`)

If these values do not match:

- The game may render internally at one resolution  
- The FOV/aspect ratio may be calculated for another  
- This results in stretching, squashing, and incorrect FOV  

# Suggestion 

It seems that the game does not like to go past 1920 x 1080 so just leave the configuration files as they are set up for you. if you change any settings it is done so at your own risk that the game may not work as intended by the fixes.

---

### Controller Support (works out of the box)

Controller support:

Works automatically — no extra configuration needed.
The game already includes native controller functionality.

Rebind controls inside the game’s options menu.

---

# Credits

- **AlphaYellow** — Widescreen & FOV Fix  
- **Elisha Riedlinger** — DXWrapper  
- **UCyborg** — Legacy D3D Resolution Hack  
- **ThirteenAG** — Ultimate ASI Loader  
- **Elisha / ThirteenAG** — D3D9 wrapper base  
- **Chip** — Installer reconstruction, registry patching, modern fix integration, resolution override tool  

---

# Issues and Support

For help or to report issues, visit the Discord server:  
https://discord.gg/eVJ7sQH7Cc

---

### Fix Enhancers  
https://fixenhancers.wixsite.com/fix-enhancers

“Creating compatibility fixes and enhancements for legacy PC games.”

# Chip
- founder
- reverse engineer
- programmer
- developer
- Game Preservationist
  
<img width="250" height="500" alt="my logoo" src="https://github.com/user-attachments/assets/9bb13d3f-0734-4f1d-b68f-14114b13744a" />


# JokerAlex21 
- founder
- admin
- tester 

<img width="250" height="250" alt="YouTube_Logo" src="https://github.com/user-attachments/assets/5c7204ca-4bca-4673-8117-965732e7ee6d" />
