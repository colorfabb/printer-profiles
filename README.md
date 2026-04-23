# colorFabb Printer Profiles

Professional 3D printing profiles for [colorFabb](https://colorfabb.com/) filaments, optimized for use with **PrusaSlicer**, **OrcaSlicer**, **SnapmakerOrca**, **BambuStudio**, **QIDIStudio**, and **AnyCubicSlicer**.

## 🎨 Supported Materials

This repository includes profiles for the following colorFabb materials:

- **PLA** - ColorFabb’s signature biobased PLA blends offer great printability with enhanced toughness and less brittleness, making them ideal for reliable everyday printing.
- **TPU** - TPU options like varioShore TPU and TPU 85A/95A offer a range from ultra-soft to semi-flexible, using innovative foaming tech to vary softness, density, and elasticity for wearable and ergonomic applications.
- **CO-POLYESTER** - The engineering-grade filament (a co-polyester) delivers clear, food-safe, low-odor prints with outstanding toughness and layer adhesion.
- **ASA** - ASA filaments are UV- and high-temperature-resistant, providing tough, rigid outdoor prints that withstand the elements.
- **PA (Nylon)** - PA filaments (like PA Neat or PA-CF Low Warp) are nylon-based, highly durable, low-warp, and built to endure elevated temperatures—perfect for functional, engineering parts.
- **PHA** - allPHA is a 100% biobased and fully biodegradable filament made via bacterial fermentation, designed to minimize environmental impact without leaving microplastics behind.

## 📦 Installation

### PrusaSlicer

1. Download the profiles from the `PrusaSlicer` directory
2. Open PrusaSlicer
3. Navigate to: **Configuration** → **Configuration Wizard** → **Custom**
4. Or manually copy files to:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\PrusaSlicer\`
   - **macOS**: `~/Library/Application Support/PrusaSlicer/`
   - **Linux (Ubuntu, native/AppImage)**: `~/.config/PrusaSlicer/`
   - **Linux (Ubuntu, Flatpak)**: `~/.var/app/com.prusa3d.PrusaSlicer/config/PrusaSlicer/user/` (default user: `.../user/default/`)

Copy the files to their respective directories:
- Filament profiles → `filament/`
- Print profiles → `print/`

### OrcaSlicer

1. Download the profiles from the `OrcaSlicer` directory
2. Open OrcaSlicer
3. Navigate to: **Configuration** → **Preferences** → **User Presets**
4. Or manually copy files to:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\OrcaSlicer\user\`
   - **macOS**: `~/Library/Application Support/OrcaSlicer/user/`
   - **Linux (Ubuntu, native/AppImage)**: `~/.config/OrcaSlicer/user/` (default user: `.../user/default/`)
   - **Linux (Ubuntu, Flatpak)**: `~/.var/app/com.orcaslicer.OrcaSlicer/config/OrcaSlicer/user/` (default user: `.../user/default/`)

On Ubuntu, these slicers typically store presets under `.../user/`. The default user is usually `.../user/default/`, but if you create/sign into an account the slicer may create an additional subfolder under `.../user/`. Copy profiles into the folder that matches your active user.

Copy the files to their respective directories:
- Filament profiles → `filament/`
- Process profiles → `process/`

### SnapmakerOrca

1. Download the profiles from the `SnapmakerOrca` directory
2. Open SnapmakerOrca
3. Find your **User Presets** location in the app settings/preferences
4. Copy the files to their respective directories under your user presets folder.

Ubuntu preset locations (AppImage/native installs):
- `~/.config/Snapmaker_Orca/user/`
- Default user: `~/.config/Snapmaker_Orca/user/default/`

If you create/sign into an account, SnapmakerOrca may create an additional subfolder under `.../user/`. Copy profiles into the folder that matches your active user.

Folder layout under your selected user folder:
   - Filament profiles → `filament/`
   - Process profiles → `process/`

Note: The profiles in `SnapmakerOrca` are a direct duplicate of `OrcaSlicer` and use the same folder layout.

### BambuStudio

1. Download the profiles from the `BambuStudio` directory
2. Open BambuStudio
3. Navigate to: **Settings** → **Preferences** → **User Presets**
4. Or manually copy files to:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\BambuStudio\user\`
   - **macOS**: `~/Library/Application Support/BambuStudio/user/`
   - **Linux (Ubuntu, native/AppImage)**: `~/.config/BambuStudio/user/` (default user: `.../user/default/`)
   - **Linux (Ubuntu, Flatpak)**: `~/.var/app/com.bambulab.BambuStudio/config/BambuStudio/user/` (default user: `.../user/default/`)

Copy the files to their respective directories:
- Filament profiles → `filament/`
- Process profiles → `process/`

### QIDIStudio

1. Download the profiles from the `QIDIStudio` directory
2. Open QIDIStudio
3. Navigate to: **Settings** → **Preferences** → **User Presets**
4. Or manually copy files to:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\QIDIStudio\user\`
   - **macOS**: `~/Library/Application Support/QIDIStudio/user/`
   - **Linux (Ubuntu, native/AppImage)**: `~/.config/QIDIStudio/user/` (default user: `.../user/default/`)

Copy the files to their respective directories:
- Filament profiles → `filament/`
- Process profiles → `process/`

### AnyCubicSlicer

1. Download the profiles from the `AnyCubicSlicer` directory
2. Open AnyCubicSlicer
3. Navigate to: **Settings** → **Preferences** → **User Presets**
4. Or manually copy files to:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\AnycubicSlicerNext\user\[user-number]\`
   - **Linux (Ubuntu, native/AppImage)**: `~/.config/AnycubicSlicerNext/user/` (default user: `.../user/default/`)
   - **Linux (Ubuntu, Flatpak)**: `~/.var/app/com.anycubic.SlicerNext/config/AnycubicSlicerNext/user/` (default user: `.../user/default/`)

   Note: the `user` directory typically contains multiple profile folders (for example a numeric folder and/or `default`). Copy the profiles into the folder that matches your active AnyCubicSlicer user profile.

Copy the files to their respective directories:
- Filament profiles → `filament/`
- Process profiles → `process/`

## 🔧 Usage

### PrusaSlicer

1. Open PrusaSlicer
2. Select a colorFabb filament profile from the **Filament** dropdown
3. Select a colorFabb print profile from the **Print Settings** dropdown
4. Adjust printer settings as needed for your specific printer

### OrcaSlicer / BambuStudio / QIDIStudio / AnyCubicSlicer

1. Open OrcaSlicer, BambuStudio, QIDIStudio, or AnyCubicSlicer
2. Select a colorFabb filament from the **Filament** dropdown
3. Select a colorFabb process profile from the **Process** dropdown
4. Configure your printer settings

## 📋 Print Settings Overview

### Recommended Print Settings

| Material                   | Nozzle Temp   | Bed Temp      | Fan Speed   | Print Speed    |
|----------------------------|---------------|---------------|-------------|----------------|
| PLA Economy                | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| PLA CoD                    | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| PLA/PHA                    | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| PLA Semi Matte             | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| PLA HP                     | 200-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| PLA Regrind                | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| PLA High Speed Pro         | 215-225°C     | 50-60°C       | 100%        | 275-285 mm/s   |
| stoneFill                  | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| corkFill                   | 210-230°C     | 50-60°C       | 100%        | 40-60 mm/s     |
| woodFill                   | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| copperFill                 | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| bronzeFill                 | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| steelFill                  | 190-210°C     | 50-60°C       | 100%        | 40-80 mm/s     |
| glowFill                   | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| Vibers                     | 195-220°C     | 50-60°C       | 100%        | 40-100 mm/s    |
| LW-PLA (Unfoamed)          | 210°C         | 50-60°C       | 100%        | 40-100 mm/s    |
| LW-PLA (Foamed)            | 235°C         | 50-60°C       | 100%        | 40-100 mm/s    |
| LW-PLA-HT (Unfoamed)       | 210°C         | 50-60°C       | 100%        | 40-100 mm/s    |
| LW-PLA-HT (Foamed)         | 235°C         | 50-60°C       | 100%        | 40-100 mm/s    |
| allPHA                     | 190-200°C     | 0-60°C        | 100%        | 40-80 mm/s     |
| varioShore TPU (Unfoamed)  | 210°C         | 20-40°C       | 100%        | 20-30 mm/s     |
| varioShore TPU (Foamed)    | 235°C         | 20-40°C       | 100%        | 20-30 mm/s     |
| TPU 85A                    | 220-230°C     | 30-40°C       | 25-50%      | 30-40 mm/s     |
| TPU 95A                    | 220-230°C     | 30-40°C       | 25-50%      | 30-40 mm/s     |
| PETG Economy               | 235-255°C     | 70-80°C       | 75-100%     | 30-50 mm/s     |
| PETG Semi Matte            | 235-255°C     | 70-80°C       | 75-100%     | 30-50 mm/s     |
| PETG Regrind               | 235-255°C     | 70-80°C       | 75-100%     | 30-50 mm/s     |
| PETG                       | 235-255°C     | 70-80°C       | 75-100%     | 30-50 mm/s     |
| colorFabb XT               | 240-260°C     | 60-70°C       | 25-50%      | 40-70 mm/s     |
| colorFabb XT CF20          | 240-260°C     | 60-70°C       | 25-50%      | 40-70 mm/s     |
| colorFabb HT               | 250-280°C     | 100-120°C     | 25-50%      | 30-50 mm/s     |
| nGen                       | 220-240°C     | 75-85°C       | 25-50%      | 40-70 mm/s     |
| nGen_flex                  | 240-260°C     | 75-85°C       | 25-50%      | 30-60 mm/s     |
| nGen CF10                  | 220-240°C     | 75-85°C       | 25-50%      | 40-70 mm/s     |
| ASA                        | 240-260°C     | 90-100°C      | 0-50%       | 30-50 mm/s     |
| LW-ASA (Foamed)            | 240°C         | 90-100°C      | 0-50%       | 30-50 mm/s     |
| PA Neat                    | 265-290°C     | 30-50°C       | 0-50%       | 30-40 mm/s     |
| PA-CF Low Warp             | 260-280°C     | 30-50°C       | 0-50%       | 30-40 mm/s     |
| PA Blue Metal Detectable   | 265-290°C     | 30-50°C       | 0-50%       | 30-40 mm/s     |

## ⚠️ Important Notes


### General Tips
- Always run a temperature tower when trying a new material
- Adjust retraction settings based on your specific printer
- Clean nozzle between material changes
- Use a brim or raft for materials with poor bed adhesion

## 🔄 Updates

These profiles are regularly updated based on:
- colorFabb material specifications
- Community feedback
- Testing with various printer models

## 📄 License

These profiles are provided as-is for use with colorFabb materials. Feel free to modify them for your specific needs.

## 🤝 Contributing

Found an issue or have a suggestion? Please open an issue or submit a pull request!

## 📞 Support

For questions about colorFabb materials:
- Visit [colorFabb.com](https://colorfabb.com/)
- Email: info@colorfabb.com

For profile-specific issues:
- Open an issue in this repository

## ⚡ Quick Start

1. Download the profiles for your slicer
2. Import them into your slicer
3. Select the colorFabb material you're using
4. Select the quality preset (0.20mm recommended)
5. Start printing!

---

**Note**: These are starting point profiles. You may need to fine-tune settings based on your specific printer, nozzle size, and environmental conditions.
