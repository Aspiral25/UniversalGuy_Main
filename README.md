# UniversalGuy Dev Hub (WAFI Dev Hub)

A central portfolio hub for web tools, documentation, and live demos. The hub provides a unified interface to browse projects, read documentation, and launch interactive applications.

## Live Site Structure

### Main Hub — `index.html`
- **Dev Hub landing page** with sidebar navigation, dark/light theme toggle, and mobile responsive layout.
- **Projects navigation** with expandable sidebar sections and live iframe previews.
- **Tab system**: Documentation panel + Live App panel for embedded tools.
- **Coffee/Ko-fi support button**.

### Projects

#### 1. Construction Material Calculator — `calculator.html`
A bilingual (Malay/English) construction estimation tool for Malaysian contractors and DIY enthusiasts.

| Module | Inputs | Outputs |
|---|---|---|
| **Wall Material** | Wall length, height, window dimensions | Bricks, cement bags, sand (ela) — construction & plaster |
| **Floor Tile** | Floor length, width | Tiles (300mm & 600mm), mortar cement, sand, adhesive cement |
| **Concrete** | Length, width, height | Volume, ready-mix cost, manual mix (cement, sand, aggregate, BRC) |
| **Paint** | Wall length/height (ft), coats, brand | Surface area, sealer litres, paint litres |

**Features:**
- Expandable formula panels on each calculator card
- Material Reference Data tab with standard densities, bag weights, and conversion factors
- Formula Reference Guide tab with every equation used
- 4-step educational guide explaining construction estimation workflow
- Bilingual interface (Malay/English) with `localStorage` persistence

#### 2. Faraid Calculator — `faraid.html`
An accurate and Syariah-compliant Islamic inheritance calculator.

**Features:**
- Estate net calculation after funeral expenses and debts
- Fixed-share heirs: Wife (1/8 with children, 1/4 without), Mother (1/6 with children, 1/3 without)
- Residuary (Asabah) distribution for children with 2:1 son-to-daughter ratio
- Visual tree breakdown showing each heir's fraction and exact RM value
- **Al-Hajb (Blocking) rules** — automatically disables inputs for blocked heirs (e.g., maternal grandma blocked by mother)
- 5 heir categories: Primary Heirs, Substitute Heirs, Siblings, Extended Relatives
- Bilingual interface (Malay/English)
- Uses `Fraction.js` for exact Islamic mathematics without floating-point rounding errors

#### 3. ERP Guide — `index.html` (embedded notes)
Detailed Q&A and workflow procedures for the Monitor G5 ERP system.

**Sections:**
- User flows for Sales & CS, Design EE, Manufacturing EE, Store, Finance
- Purchaser procedures (PO creation, subcontract, blanket orders)
- Admin tasks (system updates, licensing, agent schedulers)
- Project and PR website references

#### 4. Regex Playground — coming soon

## Tech Stack

- **Frontend**: HTML5, CSS3 (responsive grid), vanilla JavaScript
- **Math**: `Fraction.js` (Faraid calculator)
- **Deployment**: GitHub Pages — `index.html` is the Dev Hub; each tool is self-contained.

## Material Constants

| Constant | Value | Usage |
|---|---|---|
| Cement bulk density | 1440 kg/m³ | Converting volume to bag count |
| Cement bag weight | 50 kg | Standard Malaysian bag |
| Bags per m³ | 28.8 (wall/floor), 28.25 (concrete) | Mix ratio-specific |
| 1 ela | 1.308 m³ | Malaysian volumetric unit for sand |
| Brick face area | 0.22m × 0.07m (0.0154 m²) | Standard Malaysian brick |
| Tile sizes | 300×300mm (1ft), 600×600mm (2ft) | Floor tiles |
| Adhesive bag weight | 25 kg | Tile adhesive |
| BRC sheet size | 2.2m × 6m | A6 JKR Spec reinforcing mesh |
| Paint coverage | Nippon 107, Dulux 124, Jotun 113 sq ft/litre | 2-coat on primed walls |

## Formulas

All calculations follow Malaysian construction standards:
- **Wall mortar**: 30mm thickness, 1:4 cement:sand
- **Plaster**: 19mm thickness, 1:4 cement:sand
- **Concrete mix**: 1:2:2 (cement:sand:aggregate)
- **Paint**: Uses feet (not meters); sealer always 1 coat

For full breakdowns, open any calculator and switch to the **Formula Guide** tab.

## Getting Started

### Run Locally
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
pip install pyqt6
python housecal.py
```

## Screenshots / Live Demo
Deployed via GitHub Pages. Open `index.html` and navigate via the sidebar to launch each tool.

## Contributing
Contributions are welcome — feel free to open issues or submit PRs for new material types, regions, or additional estimators.

## License
MIT License. Free for personal and commercial use.
