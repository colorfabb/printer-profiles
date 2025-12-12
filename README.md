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

### Recommended Temperatures

| Material | Nozzle Temp | First Layer | Bed Temp | First Layer Bed |
|----------|-------------|-------------|----------|-----------------|
| PLA/PHA  | 205°C       | 210°C       | 60°C     | 60°C            |
| PETG     | 245°C       | 250°C       | 75°C     | 85°C            |
| nGen     | 230°C       | 235°C       | 70°C     | 85°C            |
| nGen_flex| 230°C       | 235°C       | 50°C     | 50°C            |

### Print Speed Recommendations

| Material | Outer Wall | Inner Wall | Infill | Top Layer |
|----------|-----------|------------|--------|-----------|
| PLA/PHA  | 40 mm/s   | 50 mm/s    | 60 mm/s| 40 mm/s   |
| PETG     | 40 mm/s   | 50 mm/s    | 60 mm/s| 40 mm/s   |
| nGen     | 40 mm/s   | 50 mm/s    | 60 mm/s| 40 mm/s   |
| nGen_flex| 20 mm/s   | 25 mm/s    | 30 mm/s| 20 mm/s   |

## ⚠️ Important Notes

### nGen_flex
- **Requires direct drive extruder** for best results
- Use minimal retraction (0.5mm recommended)
- Print slowly (20-30 mm/s)
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
