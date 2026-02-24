# Color Wavelength Simulator

A small, self-contained web app that maps **dominant wavelength** (in nanometers) to an approximate **perceived color**. The slider spans from ultraviolet (300 nm) through the visible spectrum to infrared (900 nm).

## Features

- **Wavelength slider** — 300–900 nm (UV → visible → IR) with labeled ticks
- **Live color display** — Current wavelength shown as RGB and hex, with a swatch and full-viewport background
- **Visibility labels** — Indicates whether the wavelength is ultraviolet, visible, deep red edge, or infrared
- **False-color UV/IR** — Optional toggle to show artificial colors for UV and IR so they’re visually distinct instead of fading to black
- **Keyboard** — Arrow keys adjust the wavelength by 1 nm
- **No build step** — Single HTML file; no dependencies

## How to run

Open the HTML file in a browser:

```bash
open color-wavelength-simulator-2.html
```

Or double-click `color-wavelength-simulator-2.html`, or drag it into a browser window. No server required.

## Technical note

The wavelength-to-RGB mapping is a **piecewise approximation** of single-wavelength (spectral) colors. Intensity fades near the typical visible boundaries (~380 nm and ~780 nm) because humans can’t see UV or IR. The result is an intuitive approximation for displays, not precision colorimetry.

## File

| File | Description |
|------|-------------|
| `color-wavelength-simulator-2.html` | Single-file app (HTML, CSS, and JavaScript) |
