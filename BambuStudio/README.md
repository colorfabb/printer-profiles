# BambuStudio Profiles for colorFabb

This directory contains filament and process profiles optimized for colorFabb materials in **BambuStudio**.

## Directory Structure

```
BambuStudio/
├── filament/     # Filament profiles (.json files)
└── process/      # Process profiles (.json files)
```

## Installation

### Option 1: Copy into the presets folder

1. Locate your BambuStudio user presets directory:
   - **Windows**: `C:\Users\[username]\AppData\Roaming\BambuStudio\user\`
   - **macOS**: `~/Library/Application Support/BambuStudio/user/`
   - **Linux**: `~/.config/BambuStudio/user/`

2. Copy the profile files:
   - Copy files from `filament/` to `[user-dir]/filament/`
   - Copy files from `process/` to `[user-dir]/process/`

3. Restart BambuStudio

### Option 2: Import through the UI

1. Open BambuStudio
2. Go to the **Filament** or **Process** tab
3. Use the preset menu (gear/settings) → **Import**
4. Select the `.json` profile(s)

## What’s Included

- **Filament profiles**: all `.json` files in `filament/` (the filenames match what you see in the preset list)
- **Process profiles**: all `.json` files in `process/` (for example, `0.20mm - colorFabb ...`)

## Notes

- Profiles use metric units (mm, °C)
- Treat these as starting points; fine-tune for your printer/environment

## Support

- For profile issues: open an issue in this repository and include BambuStudio version + printer details
- For material questions: [colorFabb.com](https://colorfabb.com/) / info@colorfabb.com

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
