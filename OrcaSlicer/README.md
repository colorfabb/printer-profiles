# OrcaSlicer Profiles for colorFabb

This directory contains filament and process profiles optimized for colorFabb materials in OrcaSlicer.

## Directory Structure

```
OrcaSlicer/
├── filament/     # Filament profiles (.json files)
└── process/      # Process settings profiles (.json files)
```

## Installation

### Method 1: Manual Installation

1. Locate your OrcaSlicer user presets directory:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\OrcaSlicer\user\`
   - **macOS**: `~/Library/Application Support/OrcaSlicer/user/`
   - **Linux**: `~/.config/OrcaSlicer/user/`

2. Copy the profile files:
   - Copy files from `filament/` to `[user-dir]/filament/`
   - Copy files from `process/` to `[user-dir]/process/`

3. Restart OrcaSlicer

### Method 2: Import Through UI

1. Open OrcaSlicer
2. Navigate to the **Filament** or **Process** tab
3. Click the gear icon next to the preset dropdown
4. Select **Import**
5. Choose the `.json` file you want to import
6. The profile will appear in the dropdown menu

## Available Profiles

### Filament Profiles

- **colorFabb PLA/PHA** (`colorFabb_PLA_PHA.json`) - Premium PLA blend
- **colorFabb PETG** (`colorFabb_PETG.json`) - Tough PETG material
- **colorFabb nGen** (`colorFabb_nGen.json`) - Amphora copolyester
- **colorFabb nGen_flex** (`colorFabb_nGen_flex.json`) - Semi-flexible TPU-like material

### Process Profiles

- **0.20mm Quality @colorFabb** - Balanced quality profile for all colorFabb materials

## Using the Profiles

1. Launch OrcaSlicer
2. Select your printer from the **Printer** dropdown
3. Select a colorFabb filament from the **Filament** dropdown
4. Select the colorFabb process profile from the **Process** dropdown
5. Load your 3D model and slice

## Key Features

### Pressure Advance
All profiles include recommended pressure advance values:
- Most materials: 0.02
- Flexible materials: 0.01

Adjust these values based on your specific printer and extruder setup.

### Retraction Settings
Optimized for each material:
- **PLA/PHA**: 0.8mm @ 40mm/s
- **PETG**: 1.0mm @ 35mm/s
- **nGen**: 1.0mm @ 35mm/s
- **nGen_flex**: 0.5mm @ 25mm/s (minimal)

### Cooling Profiles
Material-specific fan curves:
- **PLA/PHA**: Aggressive cooling (35-100%)
- **PETG**: Moderate cooling (20-50%)
- **nGen**: Moderate cooling (20-50%)
- **nGen_flex**: Higher cooling for flexible (40-80%)

## Customization

### Temperature Tuning

Run a temperature tower to find the optimal temperature for your setup:

1. Import a temperature tower model
2. Use OrcaSlicer's built-in temperature tower feature
3. Adjust the profile temperatures based on results

### Retraction Tuning

For direct drive extruders:
- Reduce retraction distance to 0.4-0.6mm
- May need to adjust retraction speed

For Bowden extruders:
- May need to increase retraction distance to 4-6mm
- Adjust based on Bowden tube length

### Flow Rate Calibration

1. Print a single-wall cube
2. Measure wall thickness
3. Adjust `filament_flow_ratio`:
   - Too thick: Decrease by 0.02-0.05
   - Too thin: Increase by 0.02-0.05

## OrcaSlicer-Specific Features

### Adaptive Pressure Advance
Enable in printer settings for automatic PA calibration.

### Arc Fitting
Can be enabled in process settings to smooth curves.

### AI-Based Features
OrcaSlicer includes AI-powered support generation and other features that work well with these profiles.

## Multi-Material Printing

When using colorFabb profiles with multi-material systems:

1. Ensure compatible materials in the same print
2. Set appropriate purge volumes between materials
3. Test purge tower settings before final print
4. Consider material compatibility (e.g., PLA + PETG may have adhesion issues)

## Troubleshooting

### First Layer Issues
- Adjust z-offset in small increments (0.01mm)
- Increase first layer flow if needed
- Verify bed leveling

### Inconsistent Extrusion
- Check filament diameter settings match your filament
- Verify extruder calibration
- Clean nozzle

### Overhang Quality
- Reduce overhang speed settings
- Increase cooling for better overhangs
- Enable overhang-specific settings

### Stringing
- Reduce temperature
- Increase retraction
- Enable z-hop for travels
- Enable "Only retract when crossing perimeters"

## Version Compatibility

These profiles are tested with:
- OrcaSlicer 1.9.0 and newer
- Compatible with various printer models

Older versions may not support all features.

## Performance Tips

1. **Adaptive Layer Height**: Use for complex models with varying detail
2. **Adaptive Cubic Infill**: Saves material while maintaining strength
3. **Arc Fitting**: Smoother curves and smaller G-code files
4. **Tree Supports**: Better for organic shapes

## Notes

- Profiles use metric units (mm, °C)
- All speeds are in mm/s
- Flow ratios are multiplicative (1.0 = 100%)
- Pressure advance values may need printer-specific tuning

## Support

For OrcaSlicer-specific issues:
- Visit [OrcaSlicer GitHub](https://github.com/SoftFever/OrcaSlicer)
- Join the OrcaSlicer Discord community

For profile issues:
- Open an issue in this repository
- Include OrcaSlicer version and printer details

For colorFabb material questions:
- Visit [colorFabb.com](https://colorfabb.com/)
- Contact: info@colorfabb.com
