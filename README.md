# Construction Material Calculator

A web-based and desktop tool to estimate construction materials for **walls, flooring, concrete, and paint**. Built from a PyQt6 desktop app into a single-page web app deployable on GitHub Pages.

## Features

### Calculators
| Module | Inputs | Outputs |
|---|---|---|
| **Wall Material** | Wall length, height, window dimensions | Bricks, cement bags, sand (ela) — construction & plaster |
| **Floor Tile** | Floor length, width | Tiles needed (300mm & 600mm), cement, sand, adhesive cement |
| **Concrete** | Length, width, height | Volume, ready-mix cost, manual mix breakdown (cement, sand, aggregate, BRC) |
| **Paint** | Wall length, height, coats, brand | Surface area, sealer litres, paint litres |

### Interactive Learning
- Expandable **formula panels** on each calculator card
- **Material Reference Data** tab with standard densities, bag weights, and conversion factors
- **Formula Reference Guide** tab with every equation used
- Step-by-step explanation of how construction estimation works

## Tech Stack
- **Frontend**: HTML5, CSS3 (responsive grid), vanilla JavaScript
- **Deployment**: GitHub Pages ready — just push `index.html`

## Getting Started

### Run Locally
Simply open `index.html` in any modern web browser.

```bash
# From the repo root
# Option 1: Double-click index.html
# Option 2: Serve via Python
python -m http.server 8080
# Option 3: Serve via Node
npx serve .
```

### Python Desktop App (legacy)
The original PyQt6 desktop app is also included:

```bash
# Install dependencies
pip install pyqt6

# Run the latest version
python housecal.py
```

## Formulas & Assumptions
All calculations follow standard construction mix ratios and material constants:
- **Cement density**: 1440 kg/m³ (50 kg bags → 28.8 bags/m³)
- **Sand conversion**: 1 ela = 1.308 m³
- **Brick face area**: 0.22 m × 0.07 m
- **Tile sizes**: 300 mm × 300 mm (1ft), 600 mm × 600 mm (2ft)
- **Wall mortar thickness**: 30 mm (1:4 cement:sand)
- **Plaster thickness**: 19 mm (1:4 cement:sand)
- **Concrete mix**: 1:2:2 (cement:sand:aggregate)
- **Paint coverage**: Nippon 107, Dulux 124, Jotun 113 sq ft/litre

For a full breakdown, open the web app and switch to the **Formula Guide** and **Material Data** tabs.

## Deployment

Deploy `index.html` on GitHub Pages:

1. Push this repository to GitHub
2. Go to **Settings → Pages**
3. Select **Deploy from a branch** → choose `main` (or `master`)
4. Your calculator will be live at `https://<username>.github.io/<repo-name>/`

No build step or server required.

## Screenshots / Live Demo
*(Add your deployed GitHub Pages link here)*

## Contributing
Contributions are welcome — feel free to open issues or submit PRs for new material types, regions, or additional estimators.

## License
MIT License. Free for personal and commercial use.

---

## Support

If you found this tool useful, consider buying me a coffee:

<a href="https://ko-fi.com/YOUR_KOFI_USERNAME" target="_blank">
  <img src="https://storage.ko-fi.com/cdn/kofi2.png" alt="Buy me a coffee" style="height: 60px;">
</a>

Replace `YOUR_KOFI_USERNAME` with your actual Ko-fi username.
