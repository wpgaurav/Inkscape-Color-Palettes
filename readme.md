# Inkscape Color Palettes

A curated collection of color palettes for Inkscape and GIMP. These palettes use the standard GIMP Palette format (`.gpl`) which is compatible with both applications.

## Available Palettes

| Palette | Colors | Description |
|---------|--------|-------------|
| **Google-Material.gpl** | 140+ | Complete Google Material Design color system with all primary colors and accent variants (50-900 shades + A100-A700) |
| **Material_Design.gpl** | 190+ | Comprehensive Material Design palette organized by color families with grayscale and dividers |
| **Android-icon-palette.gpl** | 15 | Essential colors optimized for Android icon design |

## Installation

### Linux

Copy the `.gpl` files to your Inkscape palettes directory:

```bash
# For Inkscape 1.0+
cp *.gpl ~/.config/inkscape/palettes/

# For older versions
cp *.gpl ~/.config/Inkscape/palettes/
```

If the directory doesn't exist, create it first:

```bash
mkdir -p ~/.config/inkscape/palettes/
```

### macOS

```bash
cp *.gpl ~/Library/Application\ Support/org.inkscape.Inkscape/config/inkscape/palettes/
```

Or navigate to `~/Library/Application Support/org.inkscape.Inkscape/config/inkscape/palettes/` in Finder and copy the files manually.

### Windows

Copy the `.gpl` files to:

```
C:\Users\<YourUsername>\AppData\Roaming\inkscape\palettes\
```

Or press `Win + R`, type `%APPDATA%\inkscape\palettes\` and press Enter, then paste the files.

### GIMP

For GIMP users, copy the palette files to:

- **Linux:** `~/.config/GIMP/2.10/palettes/`
- **macOS:** `~/Library/Application Support/GIMP/2.10/palettes/`
- **Windows:** `C:\Users\<YourUsername>\AppData\Roaming\GIMP\2.10\palettes\`

## Usage

1. Install the palette files as described above
2. Restart Inkscape (or GIMP)
3. Open the Swatches panel:
   - **Inkscape:** `View` → `Swatches` (or press `Shift + Ctrl + W`)
   - **GIMP:** `Windows` → `Dockable Dialogs` → `Palettes`
4. Select your desired palette from the dropdown menu at the bottom of the Swatches panel

## Palette File Format

These palettes use the GIMP Palette format (`.gpl`), a simple text-based format:

```
GIMP Palette
Name: My Palette
Columns: 16
#
255 128   0    FF8000    Orange
  0 128 255    0080FF    Sky Blue
```

Each color line contains:
- RGB values (0-255)
- Optional hex code
- Optional color name

## Creating Your Own Palette

1. Create a new text file with the `.gpl` extension
2. Add the header:
   ```
   GIMP Palette
   Name: Your Palette Name
   Columns: 16
   #
   ```
3. Add colors, one per line: `R G B [HexCode] [ColorName]`
4. Save and copy to the palettes directory

## Contributing

Contributions are welcome! To add a new palette:

1. Fork this repository
2. Add your `.gpl` file(s) to the root directory
3. Use descriptive filenames (e.g., `Brand-Name-Colors.gpl`)
4. Submit a pull request with a brief description of the palette

### Guidelines

- Ensure palette files are properly formatted
- Include meaningful color names where possible
- Test that the palette loads correctly in Inkscape
- Avoid duplicate or very similar palettes

## Resources

- [Inkscape Official Website](https://inkscape.org/)
- [Material Design Color System](https://material.io/design/color/)
- [GIMP Palette Documentation](https://docs.gimp.org/en/gimp-concepts-palettes.html)

## License

These color palettes are provided for free use. Material Design colors are from Google's Material Design system. Individual palette contributions may have their own attributions.

---

**Have a great palette to share?** Fork this repo and submit a pull request!
