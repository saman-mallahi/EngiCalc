# EngiCalc — Engineering Calculator & Math Studio

A single-file, browser-based engineering calculator with unit conversion, symbolic algebra (CAS), and 2D/3D plotting. Everything runs client-side — no build step, no backend, no dependencies.

> **Built with the help of AI** (Anthropic's Claude). The design, the CAS parser, the numeric solver, the 2D/3D plot engines, and the unit database were developed in a human–AI pairing session. See [Made with AI](#made-with-ai) below.

---

## ✨ Features

### 🧮 Calculator
- Scientific, Basic, Programmer, and Statistics modes
- DEG / RAD toggle
- Full expression parser (implicit multiplication, factorials, percentages)
- 40-entry history with click-to-reuse
- Programmer converter (decimal / binary / octal / hex, with `0x`, `0b`, `0o` literals)
- Statistics: mean, median, range, population & sample standard deviation

### 🔄 Unit Converter
- **85+ unit groups** across mechanics, fluids, thermal, electrical, magnetism, chemistry, photometry, radiation, and materials
- Temperature handled with proper affine conversions (°C, °F, K, °R, °Ré)
- Live filtering by name or symbol
- Click any result row to copy it to the clipboard
- Grouped navigation (Geometry & Motion, Mechanical & Fluids, Thermal & Energy, etc.)

### ✦ Math Studio
- **Expression box** with a cursor-aware sidebar keyboard (numbers, variables, constants, roots, trig, logs, number tools)
- **Examples** chips and inline syntax reference at the top
- **Tools**:
  - Simplify
  - Expand
  - Factor
  - Differentiate (1st & 2nd derivative)
  - Integrate (basic symbolic rules)
  - Solve (symbolic for polynomials up to cubic, numeric root finding otherwise)
  - Substitute / Evaluate
  - Table of values
  - 2D draw
  - 3D draw
- **Solution box** shows the answer and mirrors the latest plot
  - 3D plots: drag to rotate, scroll to zoom, "reset view" button
  - Solution and plot clear automatically when you start editing the expression
- **CAS history** — click a row to restore the input and its result
- Unicode-tolerant parser (`·`, `×`, `÷`, `−`, `–`, `—`, fullwidth punctuation)

---

## 🚀 Quick Start

### Option 1 — Just open it
Download `index.html` and open it in any modern browser (Chrome, Firefox, Safari, Edge). That's it.

### Option 2 — Run locally with a static server
```bash
# Python 3
python -m http.server 8000

# or Node
npx serve .