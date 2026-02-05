# Quick Start Guide

Get started with colorFabb printer profiles in 5 minutes!

## 🚀 Fast Installation

### PrusaSlicer
1. Download [PrusaSlicer profiles](./PrusaSlicer)
2. Copy `.ini` files to your PrusaSlicer config folder
3. Restart PrusaSlicer
4. Select colorFabb profiles from dropdowns

### OrcaSlicer
1. Download [OrcaSlicer profiles](./OrcaSlicer)
2. Copy `.json` files to your OrcaSlicer user folder
3. Restart OrcaSlicer
4. Select colorFabb profiles from dropdowns

### BambuStudio
1. Download [BambuStudio profiles](./BambuStudio)
2. Copy `.json` files to your BambuStudio user folder
3. Restart BambuStudio
4. Select colorFabb profiles from dropdowns

### AnyCubicSlicer
1. Download [AnyCubicSlicer profiles](./AnyCubicSlicer)
2. Copy `.json` files to your AnyCubicSlicer user folder
3. Restart AnyCubicSlicer
4. Select colorFabb profiles from dropdowns

## 📍 Config Locations

### Windows
- PrusaSlicer: `C:\Users\[username]\AppData\Roaming\PrusaSlicer\`
- OrcaSlicer: `C:\Users\[username]\AppData\Roaming\OrcaSlicer\user\`
- BambuStudio: `C:\Users\[username]\AppData\Roaming\BambuStudio\user\`
- AnyCubicSlicer: `C:\Users\[username]\AppData\Roaming\AnycubicSlicerNext\user\[user-number]\`

### macOS
- PrusaSlicer: `~/Library/Application Support/PrusaSlicer/`
- OrcaSlicer: `~/Library/Application Support/OrcaSlicer/user/`
- BambuStudio: `~/Library/Application Support/BambuStudio/user/`

### Linux
- PrusaSlicer: `~/.config/PrusaSlicer/`
- OrcaSlicer: `~/.config/OrcaSlicer/user/`
- BambuStudio: `~/.config/BambuStudio/user/`

## 🎯 First Print Checklist

- [ ] Profile installed in slicer
- [ ] Correct filament profile selected
- [ ] Bed cleaned with isopropyl alcohol
- [ ] Bed properly leveled
- [ ] Correct nozzle size (0.4mm default)
- [ ] Filament loaded and flowing
- [ ] Temperature tower printed (optional but recommended)

## ⚡ Quick Settings Reference

### PLA/PHA
- **Nozzle**: 205°C (first layer 210°C)
- **Bed**: 60°C
- **Speed**: 50-80 mm/s

### PETG
- **Nozzle**: 245°C (first layer 250°C)
- **Bed**: 75°C (first layer 85°C)
- **Speed**: 40-60 mm/s

### nGen
- **Nozzle**: 230°C (first layer 235°C)
- **Bed**: 70°C (first layer 85°C)
- **Speed**: 40-60 mm/s

### nGen_flex
- **Nozzle**: 230°C (first layer 235°C)
- **Bed**: 50°C
- **Speed**: 20-30 mm/s
- **Note**: Requires direct drive extruder

## 🔧 Common Issues & Fixes

### Poor Bed Adhesion
✅ Clean bed with IPA  
✅ Increase bed temp by 5°C  
✅ Add brim or raft  
✅ Check bed leveling

### Stringing
✅ Reduce temp by 5°C  
✅ Increase retraction  
✅ Enable z-hop  

### Under-extrusion
✅ Increase flow by 2-5%  
✅ Check for clogs  
✅ Verify filament diameter

### Over-extrusion
✅ Decrease flow by 2-5%  
✅ Calibrate e-steps  
✅ Check nozzle size setting

## 📚 Need More Help?

- Read the full [README.md](./README.md)
- Check slicer-specific guides:
  - [PrusaSlicer Guide](./PrusaSlicer/README.md)
  - [OrcaSlicer Guide](./OrcaSlicer/README.md)
  - [BambuStudio Guide](./BambuStudio/README.md)
  - [AnyCubicSlicer Guide](./AnyCubicSlicer/README.md)
- Visit [colorFabb.com](https://colorfabb.com/)
- Open an issue in this repository

## 🎨 Profile Customization

Start with these profiles and adjust:
1. Print a test object
2. Note any issues
3. Make small adjustments (±5°C, ±5 mm/s)
4. Test again
5. Save custom profile when satisfied

## ⏱️ Expected Print Times

With 0.20mm layer height profile:
- **Small part** (20mm cube): ~15-20 minutes
- **Benchy**: ~2-2.5 hours
- **Large part** (100x100x100mm): ~8-12 hours

Times vary based on infill, supports, and specific settings.

## 🔥 Temperature Tower

Before a big print, run a temperature tower:
1. Download a temperature tower model
2. Slice with your slicer's temperature tower feature
3. Print and observe results
4. Select the best temperature
5. Update your profile

Recommended ranges:
- PLA/PHA: 190-220°C
- PETG: 230-260°C
- nGen: 220-245°C
- nGen_flex: 220-245°C

---

**Happy Printing! 🎉**
