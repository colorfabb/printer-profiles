# PrusaSlicer Profiles for colorFabb

This directory contains filament and print profiles optimized for colorFabb materials in PrusaSlicer.

## Directory Structure

```
PrusaSlicer/
├── filament/     # Filament profiles (.ini files)
└── print/        # Print settings profiles (.ini files)
```

## Installation

### Method 1: Manual Installation

1. Locate your PrusaSlicer configuration directory:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\PrusaSlicer\`
   - **macOS**: `~/Library/Application Support/PrusaSlicer/`
   - **Linux**: `~/.config/PrusaSlicer/`

2. Copy the profile files:
   - Copy files from `filament/` to `[config-dir]/filament/`
   - Copy files from `print/` to `[config-dir]/print/`

3. Restart PrusaSlicer

### Method 2: Import Through UI

1. Open PrusaSlicer
2. Go to **File** → **Import** → **Import Config**
3. Select the `.ini` files you want to import
4. Profiles will appear in the respective dropdown menus

## Available Profiles

### Filament Profiles

- **colorFabb PLA/PHA** - Premium PLA with enhanced properties
- **colorFabb PETG** - Tough, chemical-resistant PETG
- **colorFabb nGen** - Amphora-based copolyester
- **colorFabb nGen_flex** - Semi-flexible material (Shore 95A)

### Print Profiles

- **0.20mm QUALITY @colorFabb** - Balanced quality and speed

## Using the Profiles

1. Launch PrusaSlicer
2. Select your printer from the **Printer** dropdown
3. Select a colorFabb filament from the **Filament** dropdown
4. Select a print profile from the **Print Settings** dropdown
5. Load your 3D model and slice

## Customization

These profiles are starting points. You may need to adjust:

- **Temperatures**: Run a temperature tower for your specific printer
- **Retraction**: Adjust based on your extruder type (Bowden vs. Direct Drive)
- **Speeds**: Modify based on your printer's capabilities
- **Cooling**: Fine-tune for your part geometry

## Profile Inheritance

These profiles can be used as base profiles for creating custom configurations:

1. Right-click on a profile in PrusaSlicer
2. Select **Duplicate**
3. Modify settings as needed
4. Save with a new name

## Troubleshooting

### Poor bed adhesion
- Increase first layer bed temperature by 5°C
- Clean bed with isopropyl alcohol
- Use brim or raft
- Level bed properly

### Stringing
- Decrease temperature by 5°C
- Increase retraction distance
- Increase retraction speed
- Enable "Wipe while retracting"

### Layer separation
- Increase nozzle temperature by 5°C
- Reduce cooling fan speed
- Slow down print speed
- Check for drafts affecting the print

### Over-extrusion
- Calibrate E-steps
- Reduce extrusion multiplier by 0.05
- Check filament diameter

### Under-extrusion
- Increase extrusion multiplier by 0.05
- Check for nozzle clogs
- Verify filament diameter
- Check for filament tangles

## Version Compatibility

These profiles are tested with:
- PrusaSlicer 2.6.0 and newer
- SuperSlicer 2.5.0 and newer (compatible fork)

## Notes

- Always perform a test print when using new profiles
- Profile settings are conservative for reliability
- Adjust for your specific printer and environment
- Keep nozzle clean for best results

## Support

For issues with these profiles:
- Open an issue in the main repository
- Include your PrusaSlicer version and printer model
- Provide photos of print issues

For colorFabb material questions:
- Visit [colorFabb.com](https://colorfabb.com/)
- Contact: info@colorfabb.com
