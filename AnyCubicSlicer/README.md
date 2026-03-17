# AnyCubicSlicer Profiles for colorFabb

This directory contains filament and process profiles optimized for colorFabb materials in **AnyCubicSlicer**.

AnyCubicSlicer uses the same preset format as **OrcaSlicer** and **BambuStudio**, so these profiles use the same folder layout and preset format.

## Directory Structure

```
AnyCubicSlicer/
├── filament/     # Filament profiles (.json files)
└── process/      # Process settings profiles (.json files)
```

## Installation

### Option 1: Copy into the presets folder

1. Locate your AnyCubicSlicer user presets directory:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\AnycubicSlicerNext\user\[user-number]\`

   In this folder you will typically see multiple profile directories (for example a numeric folder like `646375` and/or `default`). Use the one that matches your active AnyCubicSlicer user profile.

2. Copy the profile files:
   - Copy files from `filament/` to `[user-dir]/filament/`
   - Copy files from `process/` to `[user-dir]/process/`

3. Restart AnyCubicSlicer

### Option 2: Import through the UI

1. Open AnyCubicSlicer
2. Navigate to the **Filament** or **Process** tab
3. Click the settings/gear icon next to the preset dropdown
4. Select **Import**
5. Choose the `.json` file you want to import
6. The profile will appear in the dropdown menu

## What’s Included

- **Filament profiles**: all `.json` files in `filament/`
- **Process profiles**: all `.json` files in `process/` (for example, `0.20mm - colorFabb ...`)

## Notes

- Profiles use metric units (mm, °C)
- All speeds are in mm/s
- These are starting point profiles; you may need to fine-tune for your specific printer and environment

## Support

For profile issues:
- Open an issue in this repository
- Include AnyCubicSlicer version and printer details

For colorFabb material questions:
- Visit [colorFabb.com](https://colorfabb.com/)
- Contact: info@colorfabb.com
