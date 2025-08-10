# Soil FTIR Absorbance Simulator

Interactive soil FTIR absorbance simulator with sliders for clays, water (interlayer & adsorbed), organic matter, nitrate, and bound orthophosphate — initialized with data from organic farms in the SUNY Oneonta area. Runs as a single offline HTML file (`index.html`).

## Features

- Component sliders: montmorillonite, kaolinite, chlorite, illite
- Water: interlayer (\~1630 cm⁻¹), adsorbed (\~3400 cm⁻¹)
- Organics: 1715, 1620, 1515, 1420, 1230, 1030 cm⁻¹
- Nitrate: 1384, 824 cm⁻¹; Bound orthophosphate: 1085, 1040, 980, 565 cm⁻¹
- Baseline offset & slope; show/hide components; normalize; reset
- Clean SVG chart (no external libraries), works fully offline

## Quick start (local)

1. Download `index.html` from this repository.
2. Double‑click to open it in your browser (Chrome/Edge/Firefox). No build step, no dependencies.


## Data / Attribution

Model initialized using FTIR data sampled from organic farms in the SUNY Oneonta area.

## How it works (high‑level)

- Each component is modeled as a sum of **Gaussian** or **Lorentzian** peaks at characteristic wavenumbers.
- The **baseline** is a linear function (offset + slope) added to the summed components.
- The **Total** trace equals baseline + all component traces, with an option to normalize to a maximum of 1.0.

## File structure

```
├── index.html   # Full simulator (HTML, CSS, JS in one file)
└── README.md    # This file
```

You may add a `LICENSE` file (MIT recommended for open educational use).

## License

MIT — see `LICENSE` in this repository (or choose a different license to suit your needs).

## Acknowledgments

- Organic farms in the SUNY Oneonta area (source region for initial spectra)
- Community users who provide feedback and peak adjustments

## Issues & contributions

Found a bug or want a new feature (e.g., export CSV/PNG, toggle “Total (no baseline)”, or additional minerals)?

1. Open an **Issue** describing the change.
2. Or fork and submit a **Pull Request**.

## Suggested repository topics

`ftir` `infrared` `spectroscopy` `soil` `geochemistry` `agronomy` `oneonta` `organic-farming` `web-simulator` `education`

