# Contributing to colorFabb Printer Profiles

Thank you for your interest in contributing to the colorFabb printer profiles repository!

## How to Contribute

### Reporting Issues

If you encounter problems with any profile:

1. **Check existing issues** first to avoid duplicates
2. **Provide detailed information**:
   - Slicer name and version
   - colorFabb material being used
   - Printer model and specifications
   - Expected vs. actual behavior
   - Photos of print issues (if applicable)

### Suggesting Improvements

Have an idea for better settings?

1. Open an issue describing the improvement
2. Explain the benefits of the change
3. Include test results if available
4. Reference specific materials and conditions

### Submitting Profile Updates

To submit updated or new profiles:

1. **Fork** this repository
2. **Create a branch** for your changes
3. **Test** your profiles thoroughly:
   - Print at least 3 test objects
   - Document your printer specifications
   - Include temperature tower results
4. **Document** your changes:
   - What was changed and why
   - Test results and observations
   - Any trade-offs or limitations
5. **Submit a pull request** with:
   - Clear description of changes
   - Test results
   - Photos of prints (optional but helpful)

## Profile Guidelines

### File Naming

- **PrusaSlicer**: Use descriptive names with spaces (e.g., `colorFabb PLA-PHA.ini`)
- **OrcaSlicer/BambuStudio**: Use underscores (e.g., `colorFabb_PLA_PHA.json`)

### Profile Standards

All profiles should include:

1. **Material Information**:
   - Correct filament type classification
   - Density and cost (approximate)
   - Vendor set to "colorFabb"

2. **Temperature Settings**:
   - Conservative defaults that work for most printers
   - Reasonable temperature ranges
   - First layer temperatures for good adhesion

3. **Speed Settings**:
   - Safe speeds that produce good quality
   - Appropriate for the material type
   - Consider maximum volumetric flow rate

4. **Cooling Settings**:
   - Appropriate for material type
   - Layer time considerations
   - Fan speeds optimized for quality

5. **Notes/Documentation**:
   - Brief material description
   - Recommended settings summary
   - Special considerations or warnings

### Testing Requirements

Before submitting profiles, please test with:

- **Calibration prints**: Temperature tower, retraction tower
- **Functional parts**: Benchy, overhang test, bridging test
- **Real-world prints**: At least one practical object

### Quality Standards

Profiles should produce prints with:

- Good layer adhesion
- Minimal stringing
- Clean overhangs (within material limits)
- Consistent extrusion
- Good first layer adhesion

## Code of Conduct

- Be respectful and constructive
- Focus on improving print quality
- Share knowledge and experience
- Help others in the community

## Questions?

If you have questions about contributing:

1. Check existing issues and discussions
2. Review the README.md
3. Open an issue with the "question" label

## Review Process

Pull requests will be reviewed for:

1. **Completeness**: All required information provided
2. **Testing**: Evidence of thorough testing
3. **Quality**: Profiles meet quality standards
4. **Documentation**: Changes are well documented
5. **Compatibility**: Works with stated slicer versions

Reviews typically take 3-7 days. We may request changes or additional testing.

## Recognition

Contributors will be acknowledged in:
- Pull request comments
- Release notes (for significant contributions)

Thank you for helping improve colorFabb printer profiles!
