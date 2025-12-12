# BambuStudio Profiles for colorFabb

This directory contains filament and process profiles optimized for colorFabb materials in BambuStudio.

## Directory Structure

```
BambuStudio/
├── filament/     # Filament profiles (.json files)
└── process/      # Process settings profiles (.json files)
```

## Installation

### Method 1: Manual Installation

1. Locate your BambuStudio user presets directory:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\BambuStudio\user\`
   - **macOS**: `~/Library/Application Support/BambuStudio/user/`
   - **Linux**: `~/.config/BambuStudio/user/`

2. Copy the profile files:
   - Copy files from `filament/` to `[user-dir]/filament/`
   - Copy files from `process/` to `[user-dir]/process/`

3. Restart BambuStudio

### Method 2: Import Through UI

1. Open BambuStudio
2. Navigate to the **Filament** or **Process** tab
3. Click the settings icon next to the preset dropdown
4. Select **Import**
5. Choose the `.json` file you want to import
6. The profile will appear in the dropdown menu

## Available Profiles

### Filament Profiles

- **colorFabb PLA/PHA** (`colorFabb_PLA_PHA.json`) - Premium PLA blend
- **colorFabb PETG** (`colorFabb_PETG.json`) - Tough PETG material
- **colorFabb nGen** (`colorFabb_nGen.json`) - Amphora copolyester
- **colorFabb nGen_flex** (`colorFabb_nGen_flex.json`) - Semi-flexible material

### Process Profiles

- **0.20mm Quality @colorFabb** - Balanced quality profile for all colorFabb materials

## Using the Profiles

1. Launch BambuStudio
2. Select your Bambu Lab printer from the **Printer** dropdown
3. Select a colorFabb filament from the **Filament** dropdown
4. Select the colorFabb process profile from the **Process** dropdown
5. Load your 3D model and slice

## Bambu Lab Printer Compatibility

These profiles work with all Bambu Lab printers:
- **X1 Series** (X1, X1 Carbon, X1E)
- **P1 Series** (P1P, P1S)
- **A1 Series** (A1, A1 mini)

### Printer-Specific Notes

#### X1 Carbon / X1
- Full chamber heating available for engineering materials
- AMS (Automatic Material System) compatible
- Use chamber heating for nGen and PETG in cold environments

#### P1 Series
- Semi-enclosed design
- AMS Lite compatible
- Good for all colorFabb materials

#### A1 Series
- Open frame design
- Single-color printing or AMS Lite
- Excellent for PLA/PHA
- Use enclosure for PETG/nGen in drafty areas

## Key Features

### Flow Calibration
BambuStudio includes automatic flow calibration:
1. Use the built-in calibration feature
2. Adjust `filament_flow_ratio` based on results
3. Save custom profile with your calibrated values

### Pressure Advance
All profiles include recommended pressure advance values:
- Most materials: 0.02
- Flexible materials: 0.01

Fine-tune using BambuStudio's PA calibration tool.

### Lidar & AI Features (X1 Series)
The X1 series lidar and AI detection work great with these profiles:
- First layer inspection
- Spaghetti detection
- Print failure detection

### AMS Multi-Color Printing

When using colorFabb filaments with AMS:

1. Load filaments in AMS slots
2. Assign each slot a colorFabb profile
3. Use appropriate purge volumes:
   - PLA to PLA: 50-70mm³
   - PLA to PETG: 100-120mm³
   - PETG to PLA: 120-150mm³
   - Similar materials: 50-70mm³

4. Enable prime tower for best color transitions

## Temperature Settings

### Recommended for Bambu Lab Printers

| Material | Nozzle | Bed | Chamber (X1) |
|----------|--------|-----|--------------|
| PLA/PHA  | 205°C  | 60°C| 0°C (off)    |
| PETG     | 245°C  | 75°C| 35°C         |
| nGen     | 230°C  | 70°C| 35°C         |
| nGen_flex| 230°C  | 50°C| 0°C (off)    |

### Hardened Nozzle Recommendations
For abrasive filaments (not included in this profile set):
- Use hardened steel or tungsten carbide nozzle
- May need +5-10°C due to lower thermal conductivity

## Speed Profiles

BambuStudio supports speed override:
- **Silent**: Use for dimensional accuracy
- **Standard**: Recommended for colorFabb profiles
- **Sport**: Good for PLA/PHA, may require tuning for others
- **Ludicrous**: PLA/PHA only, requires testing

## Customization

### Chamber Temperature (X1 Series)
Adjust for better results with engineering materials:
- PETG: 35-40°C helps with layer adhesion
- nGen: 35-40°C reduces warping
- PLA/PHA: Keep at 0°C (off) to prevent softening

### Cooling Fan Override
BambuStudio allows auxiliary fan control:
- Part cooling fan settings in filament profile
- Auxiliary fan for better overall cooling
- Chamber fan to manage temperature

## Network Printing

Send prints to Bambu Lab printers over network:

1. Ensure printer is on same network
2. Slice with colorFabb profiles
3. Send to printer via LAN or Cloud
4. Monitor via camera and app

## Cloud Storage

BambuStudio supports cloud project storage:
- Save profiles to Bambu Cloud
- Access from multiple computers
- Share profiles with team members

## Troubleshooting

### First Layer Issues on Textured PEI
- Increase z-offset by 0.02-0.05mm
- Use glue stick for PETG/nGen
- Clean plate with IPA

### AMS Filament Detection Issues
- Verify filament diameter matches profile
- Check AMS PTFE tubes for obstructions
- Update AMS firmware

### Stringing with AMS
- Increase retraction for long Bowden path
- Optimize purge tower settings
- Reduce print temperature slightly

### Build Plate Adhesion
- Use appropriate plate for material:
  - PLA/PHA: Smooth or textured PEI
  - PETG: Textured PEI or use glue stick
  - nGen: Textured PEI
  - nGen_flex: Smooth PEI

### Warping
- Enable brim for large parts
- Increase bed temperature by 5°C
- Use chamber heating (X1 series)
- Check for drafts

## Maintenance Tips

### Regular Maintenance
1. Clean nozzle before material changes
2. Wipe build plate with IPA before each print
3. Check extruder gears for debris
4. Calibrate flow rate periodically

### Material Storage
- Store filament in dry box or bags with desiccant
- colorFabb materials are hygroscopic
- Dry filament if printing issues occur:
  - PLA/PHA: 50°C for 4-6 hours
  - PETG: 65°C for 4-6 hours
  - nGen: 60°C for 4-6 hours

## Advanced Features

### Adaptive Layer Height
Use for better surface quality:
1. Enable in process settings
2. Set min/max layer heights
3. Adjust smoothing radius

### Support Painting
BambuStudio's support painting works well:
1. Use "Paint-on supports" for complex parts
2. Combine with tree supports for efficiency
3. Adjust support interface settings per material

### Fuzzy Skin
Available for textured surface finish:
- Works best with PLA/PHA
- Adjust thickness for desired effect

## Version Compatibility

These profiles are tested with:
- BambuStudio 1.9.0 and newer
- Compatible with all Bambu Lab printer firmware versions

## Performance Optimization

1. **Use LAN mode** for faster file transfer
2. **Enable hardware acceleration** in preferences
3. **Multi-threading** is enabled by default
4. **Limit preview quality** if slicing is slow

## Notes

- Profiles optimized for 0.4mm nozzle
- Works with other nozzle sizes with adjustments
- All temperatures are conservative starting points
- Flow rates may vary by printer and nozzle

## Support

For BambuStudio-specific issues:
- Visit [Bambu Lab Wiki](https://wiki.bambulab.com/)
- Join Bambu Lab official Discord
- Check Bambu Lab forum

For profile issues:
- Open an issue in this repository
- Include printer model and BambuStudio version

For colorFabb material questions:
- Visit [colorFabb.com](https://colorfabb.com/)
- Contact: info@colorfabb.com

## Safety Notes

- Never leave printer unattended with new profiles
- Monitor first few layers of new material
- Use proper ventilation, especially with PETG
- Keep hot parts away from flammable materials
