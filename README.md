# 🚀 UniversalGuy Dev Hub

Welcome to the **UniversalGuy Dev Hub**! 👋 This is my central portfolio hub—a unified space where you can browse my web projects, read documentation, and launch interactive applications all from one place. 

Whether you're estimating materials for a construction project, calculating inheritance, or reading up on ERP workflows, everything is just a click away.

---

## 🏠 The Main Hub (`index.html`)

The landing page acts as your dashboard. I've designed it to be as seamless and user-friendly as possible:
*   **Sleek Navigation:** An expandable sidebar to easily jump between projects and live iframe previews.
*   **Theme Toggle:** Switch between Dark and Light mode to suit your eyes. 🌙 / ☀️
*   **Interactive Tab System:** Effortlessly toggle between reading the Documentation panel and playing with the Live App panel.
*   **Fully Responsive:** Looks great whether you're on a desktop or your mobile phone.

---

## 🛠️ Featured Projects

### 🧱 1. Construction Material Calculator (`calculator.html`)
A bilingual (Malay/English) estimation tool built specifically for Malaysian contractors, builders, and DIY enthusiasts. Takes the guesswork out of your material runs!

| Construction Module | What You Input | What It Calculates |
| :--- | :--- | :--- |
| **Wall Material** | Length, height, window dimensions | Bricks, cement bags, and sand (ela) for construction & plastering. |
| **Floor Tile** | Floor length & width | Tile count (300mm/600mm), mortar cement, sand, and adhesive cement. |
| **Concrete** | Length, width, height | Total volume, ready-mix cost, and manual mix breakdown (cement, sand, aggregate, BRC). |
| **Paint** | Wall dimensions (ft), coats, brand | Surface area, sealer required (Litres), paint required (Litres). |

**✨ Key Features:**
*   **Transparent Math:** Expandable formula panels on every card, plus a dedicated **Formula Reference Guide** tab.
*   **Data at a Glance:** A Material Reference Data tab detailing standard densities, bag weights, and local conversion factors.
*   **Educational:** Built-in 4-step guide explaining the construction estimation workflow.
*   **Smart Memory:** Remembers your Malay/English preference using `localStorage`.

### ⚖️ 2. Faraid Calculator (`faraid.html`)
A highly accurate, Syariah-compliant Islamic inheritance calculator. 

**✨ Key Features:**
*   **Net Estate Calculation:** Automatically deducts funeral expenses and debts before distribution.
*   **Al-Hajb (Blocking) Rules:** Smart logic automatically disables inputs for heirs who are blocked by others (e.g., maternal grandmother blocked by mother).
*   **Flawless Math:** Powered by `Fraction.js` to ensure exact Islamic mathematics without the headache of floating-point rounding errors.
*   **Visual Breakdown:** Displays a beautiful visual tree showing each heir's fraction and their exact RM value.
*   **Comprehensive:** Covers 5 categories: Primary Heirs, Substitute Heirs, Siblings, and Extended Relatives.

### 🏢 3. ERP Guide (Embedded Notes)
Detailed Q&A and workflow procedures for the Monitor G5 ERP system.
*   **Workflows:** Covers Sales & CS, Design EE, Manufacturing EE, Store, and Finance departments.
*   **Procedures:** Step-by-step guides for Purchasers (POs, subcontracting, blanket orders) and Admins (updates, licensing, agent schedulers).

### 🔍 4. Regex Playground
*Coming soon!* 🚧

---

## 💻 Tech Stack

Keeping it fast, clean, and dependency-light:
*   **Frontend:** HTML5, CSS3 (responsive grid), Vanilla JavaScript
*   **Math Engine:** `Fraction.js` (for Faraid inheritance logic)
*   **Deployment:** GitHub Pages (Self-contained, serverless architecture)

---

## 📐 Malaysian Construction Standards & Formulas

All calculations in the Construction app strictly follow local Malaysian building standards:
*   **Wall Mortar:** 30mm thickness, 1:4 cement to sand ratio.
*   **Plaster:** 19mm thickness, 1:4 cement to sand ratio.
*   **Concrete Mix:** 1:2:2 (cement:sand:aggregate).
*   **Paint:** Calculated in square feet; sealer is always mapped to 1 coat.

### Material Constants Cheat Sheet
| Material | Standard Value | Application |
| :--- | :--- | :--- |
| **Cement** | Bulk density: 1440 kg/m³ <br>Bag weight: 50 kg | Converting total volume to physical bag counts |
| **Sand (Ela)**| 1 ela = 1.308 m³ | Malaysian volumetric unit |
| **Bricks** | 0.22m × 0.07m (0.0154 m²) | Standard Malaysian brick face area |
| **Tiles** | 300×300mm (1ft) or 600×600mm (2ft) | Standard floor tile sizes |
| **Adhesive** | 25 kg bag | Standard tile adhesive packaging |
| **BRC Mesh** | 2.2m × 6m | A6 JKR Spec reinforcing mesh |
| **Paint** | Nippon (107), Dulux (124), Jotun (113) sq ft/L | Assumes a 2-coat finish on primed walls |

---

## 🚀 Getting Started

Want to run this locally? It's incredibly simple!

### 1. Run the Web Hub
Because it's built with pure HTML/JS, you can simply double-click `index.html` to open it in your browser. Alternatively, you can spin up a local server from the repo root:

```bash
# Option A: Serve via Python
python -m http.server 8080

# Option B: Serve via Node
npx serve .
```

### 2. Run the Desktop App (Legacy)
If you prefer a native desktop experience, I've also included my original **PyQt6** Python application!

```bash
# Install PyQt6
pip install pyqt6

# Run the app
python housecal.py
```

---

## 🤝 Contributing

Contributions are always welcome! Whether you want to add new material types, support for different regional standards, or entirely new estimator tools, feel free to open an Issue or submit a Pull Request. Let's build something cool together!

## 📄 License

This project is licensed under the **MIT License**. It is completely free for personal and commercial use. 

---

## ☕ Support the Project

If you found these tools useful, saved some time on a project, or just want to say thanks, consider buying me a coffee. It keeps the caffeine flowing and the code compiling!

<a href="https://ko-fi.com/nsdotmy" target="_blank">
  <img src="https://storage.ko-fi.com/cdn/kofi2.png" alt="Buy me a coffee" style="height: 60px;">
</a>