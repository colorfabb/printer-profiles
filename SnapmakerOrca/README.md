# SnapmakerOrca Profiles for colorFabb

This directory contains filament and process profiles optimized for colorFabb materials in **SnapmakerOrca**.

These profiles are a direct duplicate of the ones in `OrcaSlicer/`.

## Directory Structure

```
SnapmakerOrca/
├── filament/     # Filament profiles (.json files)
└── process/      # Process profiles (.json files)
```

## Installation

### Option 1: Copy into the presets folder

1. In SnapmakerOrca, find where **User Presets** are stored (Settings/Preferences).
2. Copy the profile files into the matching subfolders:
   - Copy files from `filament/` to `[user-dir]/filament/`
   - Copy files from `process/` to `[user-dir]/process/`
3. Restart SnapmakerOrca

### Option 2: Import through the UI

1. Open SnapmakerOrca
2. Go to the **Filament** or **Process** tab
3. Use the preset menu (gear/settings) → **Import**
4. Select the `.json` profile(s)

## What’s Included

- **Filament profiles**: all `.json` files in `filament/`
- **Process profiles**: all `.json` files in `process/` (for example, `0.20mm - colorFabb ...`)

## Notes

- Profiles use metric units (mm, °C)
- Treat these as starting points; fine-tune for your printer/environment

## Support

- For profile issues: open an issue in this repository and include SnapmakerOrca version + printer details
- For material questions: [colorFabb.com](https://colorfabb.com/) / info@colorfabb.com
