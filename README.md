# colorFabb Printer Profiles

Professional 3D printing profiles for [colorFabb](https://colorfabb.com/) filaments, optimized for use with **PrusaSlicer**, **OrcaSlicer**, and **BambuStudio**.

## 🎨 Supported Materials

This repository includes profiles for the following colorFabb materials:

- **PLA/PHA** - Premium PLA with improved impact strength
- **PETG** - Excellent layer adhesion and chemical resistance
- **nGen** - Amphora-based copolyester with high toughness
- **nGen_flex** - Semi-flexible material (Shore 95A)

## 📦 Installation

### PrusaSlicer

1. Download the profiles from the `PrusaSlicer` directory
2. Open PrusaSlicer
3. Navigate to: **Configuration** → **Configuration Wizard** → **Custom**
4. Or manually copy files to:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\PrusaSlicer\`
   - **macOS**: `~/Library/Application Support/PrusaSlicer/`
   - **Linux**: `~/.config/PrusaSlicer/`

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
   - **Linux**: `~/.config/OrcaSlicer/user/`

Copy the files to their respective directories:
- Filament profiles → `filament/`
- Process profiles → `process/`

### BambuStudio

1. Download the profiles from the `BambuStudio` directory
2. Open BambuStudio
3. Navigate to: **Settings** → **Preferences** → **User Presets**
4. Or manually copy files to:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\BambuStudio\user\`
   - **macOS**: `~/Library/Application Support/BambuStudio/user/`
   - **Linux**: `~/.config/BambuStudio/user/`

Copy the files to their respective directories:
- Filament profiles → `filament/`
- Process profiles → `process/`

## 🔧 Usage

### PrusaSlicer

1. Open PrusaSlicer
2. Select a colorFabb filament profile from the **Filament** dropdown
3. Select a colorFabb print profile from the **Print Settings** dropdown
4. Adjust printer settings as needed for your specific printer

### OrcaSlicer / BambuStudio

1. Open OrcaSlicer or BambuStudio
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

### nGen_flex
- **Requires direct drive extruder** for best results
- Use minimal retraction (0.5mm recommended)
- Print slowly (30-60 mm/s)
- Disable retraction on travel moves if possible

### PETG and nGen
- Reduce cooling compared to PLA
- First layer bed temperature is higher for better adhesion
- May require z-offset adjustment

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
