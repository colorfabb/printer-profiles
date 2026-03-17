# PrusaSlicer Profiles for colorFabb

This directory contains filament and print profiles optimized for colorFabb materials in **PrusaSlicer**.

## Directory Structure

```
PrusaSlicer/
├── filament/     # Filament profiles (.ini files)
└── print/        # Print settings profiles (.ini files)
```

## Installation

### Option 1: Copy into the config folder

1. Locate your PrusaSlicer configuration directory:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\PrusaSlicer\`
   - **macOS**: `~/Library/Application Support/PrusaSlicer/`
   - **Linux**: `~/.config/PrusaSlicer/`

2. Copy the profile files:
   - Copy files from `filament/` to `[config-dir]/filament/`
   - Copy files from `print/` to `[config-dir]/print/`

3. Restart PrusaSlicer

### Option 2: Import through the UI

1. Open PrusaSlicer
2. Go to **File** → **Import** → **Import Config**
3. Select the `.ini` profile file(s)

## What’s Included

- **Filament profiles**: all `.ini` files in `filament/`
- **Print profiles**: all `.ini` files in `print/` (for example, `0.20mm - colorFabb ... - Prusa.ini`)

## Notes

- Profiles use metric units (mm, °C)
- Treat these as starting points; fine-tune for your printer/environment

## Support

- For profile issues: open an issue in this repository and include PrusaSlicer version + printer details
- For material questions: [colorFabb.com](https://colorfabb.com/) / info@colorfabb.com
