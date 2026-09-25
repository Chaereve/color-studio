# 🎨 Chaereve ColorLab — User Guide

A tool to view, mix, and export Photoshop (`.aco`) color palettes right in your browser.
**No installation, no data upload** — everything runs locally on your device.

---

## Table of contents
1. [Getting started](#1-getting-started)
2. [Language](#2-language)
3. ["View ACO" tab](#3-view-aco-tab)
4. ["Mix colors" tab](#4-mix-colors-tab)
5. ["Random colors" tab](#5-random-colors-tab)
6. [Design tools — Create & Analyze](#6-design-tools--create--analyze)
7. [Batch processing](#7-batch-processing)
8. [Gradient (.grd) tab](#8-gradient-grd-tab)
9. [Settings](#9-settings)
10. [Export image & data](#10-export-image--data)
11. [Mix history](#11-mix-history)
12. [Install as an app (PWA)](#12-install-as-an-app-pwa)
13. [FAQ](#13-faq)

---

## 1. Getting started

- Open `index.html` in any browser (Chrome, Edge, Firefox, Safari…).
- There are **4 tab groups** at the top:
  - **View** — open, search, edit and export colors from a `.aco` / `.grd` file.
  - **Create** — color mixer, random colors, harmony palettes, gradient builder, image → palette, built-in palettes.
  - **Analyze** — contrast checker, color-blind simulation, accessibility audit, palette statistics.
  - **Files** — merge multiple `.aco` files, open and edit Photoshop `.grd` gradients.
- The **VI / EN** control in the header switches language instantly.
- A **⚙️ Settings** button (top-right) opens the settings panel — language, font size, clear data and About.

---

## 2. Language

- Open **⚙️ Settings** (top-right) and choose a language from the **Language** menu: Vietnamese, English, 中文 (简体), 한국어, 日本語, Español.
- The whole interface switches instantly and your choice is remembered the next time you open the app.

---

## 3. "View ACO" tab

### Open a file
- **Drag & drop** a `.aco` file onto the center area, **or** click it to choose a file.
- Supports ACO **v1 and v2**, reads **color names** and the RGB / HSB / CMYK / Lab / Grayscale color spaces.

### View colors
- Each color is shown as a card: **index number** (1, 2, 3…), a swatch, name, HEX, RGB and its original color space.
- The index follows the **order in the ACO file** for easy cross-reference.

### Copy color codes
- **Click a swatch** to copy its code (choose the format — HEX / RGB / HSL — in the format menu on the toolbar).
- **📋 Copy all** copies everything as a HEX list, CSS variables, SCSS, JSON, or RGB.

### Select multiple colors
- Click the **✓** in the corner of a card to select/deselect.
- **☑ Select** → Select all / Deselect all / Invert.

### Search & sort
- **🔍** search by name, HEX or RGB.
- Sort by original order, hue, lightness, saturation, or name.

### Advanced search
Type special tokens in the search box to filter precisely:
- `hue:0-60` — colors whose hue is in that range (e.g. reds/yellows).
- `hue:>200` / `hue:<40` / `hue:120` — greater than, less than, or exact hue.
- `sat:>50` — saturation above 50; `light:40-80` — lightness between 40 and 80.
- `similar:#FF0000` — colors close to that color (RGB distance ≤ 80).
- Normal words still work; you can combine several tokens.

### Edit the palette
- **✏️ Rename** a color inline, **🗑 delete** one, or **➕ add** a new color.
- Use **↩ Undo / ↪ Redo** to step backward/forward (up to 60 steps).
- **Right-click** a swatch for a quick menu: copy, details, rename, export one color as `.aco`, or delete.
- **💾 Save .aco** writes your edits back to a new `.aco` file.

### Share palette
- Click **🔗 Share** (in the toolbar) to copy a link like `…?palette=…`.
- Opening that link loads the same palette — no server or account needed.

---

## 4. "Mix colors" tab

This tab works **standalone** — no need to open an ACO file first.

### Add colors to the mix
Two ways:
1. **Color picker** + **➕ Add this color** — choose any color.
2. **📁 Open ACO file** — pick a `.aco`, then a **selection grid** appears:
   - All colors are selected (✓) by default.
   - **Click a swatch** to exclude colors you **don't want to mix**.
   - **Select all / Deselect / Invert** buttons.
   - Click **➕ Add N colors to mix** to add the chosen colors.

### Re-adjust colors without re-uploading
- Click **🔁 Re-adjust colors** to **reopen the selection grid of the loaded ACO** (no re-upload needed).
- Tick/untick, then click "Add colors to mix" — the app **adds the new colors and removes the ones you unticked**.

### Color ratio
- The ratio is **auto-equalized** by color count (e.g. 4 colors → 25% each).
- **⚖️ Equalize ratio** resets it at any time.
- **Drag a slider** to raise/lower a single color — the rest recalculates to total 100%.

### Mix result
- The result box shows the mixed color with **HEX / RGB / HSL**, updated instantly as you change ratios.
- **📋 Copy HEX / RGB / HSL** for quick copying.
- **💾 Save to history** to keep the mixed color.

---

## 5. "Random colors" tab

Generates random colors, one per "member".

- **Mode:** 🌈 Fully random, or 🎯 By color family (red / orange / yellow / green / cyan / blue / purple / pink).
- **Number of colors** = number of members.
- **No duplicate colors** — tick to avoid repeats.
- Click **🎲 Randomize**, then **click a color card** to copy it (the number = member).
- **📋 Copy all** copies `Member #1: #XXXXXX` lines.

---

## 6. Design tools — Create & Analyze

Design tools are split across two tabs: **🧩 Create** and **🔍 Analyze**.

### 🧩 Create tab
| Tool | What it does |
|------|--------------|
| 🧩 **Palette Generator** | Creates a harmony palette (complementary, analogous, triadic, split, tetradic) from a base color. |
| 🌈 **Gradient Generator** | Builds a linear / radial / **conic** CSS gradient and copies the CSS. |
| 🖼 **Image → Palette / Eyedropper** | Click an image to pick one color, extract dominant colors, and export them straight to `.aco`. |
| 📦 **Presets & Templates** | One-click built-in palettes (Material, Tailwind, Brand Colors, Pastel, Earth Tones). |

### 🔍 Analyze tab
| Tool | What it does |
|------|--------------|
| 🔳 **Contrast Checker** | Shows the WCAG contrast ratio between text and background with AA/AAA badges. |
| 👁 **Color Blindness Preview** | Shows the palette as seen with protanopia / deuteranopia / tritanopia / grayscale. |
| ♿ **Accessibility Audit** | Percentage of the palette passing AA against white/black text. |
| 📊 **Palette Statistics** | Average saturation/lightness and a hue-distribution chart. |

Additionally, clicking **ℹ️** on any color card opens a **detail panel** with HEX / RGB / HSL / HSV / CMYK / Lab, luminance and contrast (click any row to copy).

---

## 7. Batch processing

In the **📦 Batch** tab:

- Click **Open files** and pick **several `.aco` files** at once (or drag & drop).
- The list shows each file with its color count; remove individual files with ✕.
- **Merge into Viewer** combines them into the Viewer tab (optionally removing duplicates with the "dedupe" checkbox).
- **Export merged .aco** downloads a single `merged-palette.aco`.

---

## 8. Gradient (.grd) tab

In the **📐 Gradient** tab you can open, edit and export Photoshop gradient files (`.grd`, v3 & v5).

### Open a file
- Click **📁 Open .grd file** (or drag & drop a `.grd` onto the tab) to load its gradients.
- Each gradient appears in the list with a **live preview** and a Solid/Noise badge; click one to edit it.

### Edit a solid gradient
- **Rename** it in the top field; **🗑** deletes the gradient.
- **➕ Add gradient** creates a new black→white gradient.
- **Color stops:** click a swatch to change its color, drag **Location** (0–100%) and **Midpoint** to shape the transition, **✕** removes a stop, **➕ Add color stop** inserts one in the middle.
- **Transparency stops:** same idea — Opacity and Location per stop.
- **Smoothness** controls the overall interpolation.

### Edit a noise gradient
- **Seed / 🎲 Regenerate**, **Roughness**, **Color space**, **Add transparency**, **Restrict colors**, and the **minimum / maximum** value per channel.
- Noise gradients are recreated **approximately** (Photoshop uses its own internal algorithm).

### Export
- **📋 Copy CSS** → a `linear-gradient(…)` string.
- **📐 Export SVG** → a standalone vector gradient.
- **🎨 Extract colors → .aco** → saves the color stops as a palette.
- **📁 Load into Viewer** → sends the colors to the View ACO tab.
- **💾 Save .grd** → writes all gradients back to a `.grd` file.

> **Note:** foreground/background stops are resolved to concrete colors when opened, and saved stops are always written as user stops with RGB colors.

---

## 9. Settings

The **⚙️ Settings** tab lets you personalize the app. Every choice is saved on your device.

| Setting | What it does |
|---------|--------------|
| **Language** | Choose Tiếng Việt or English. |
| **Font size** | Small / Medium / Large. |
| **Motion effects** | Turn animations on or off. |
| **Clear saved data** | Remove mix history, language, font size and all stored preferences, then reload. |
| **About** | A short description of the app. |

---

## 10. Export image & data

In the **View ACO** tab, select the colors you want, then click **⬇ Export image & data**. A dialog lets you choose:

- **Layout:** horizontal strip / vertical strip / grid (with column count).
- **Cell size** and **spacing**.
- **Label:** HEX / HEX + Name / none.
- **Background:** white or transparent.
- **Live preview** before downloading.

Export formats:

| Format | Description |
|--------|-------------|
| 🖼 PNG | High-resolution palette image |
| 📐 SVG | Vector, editable |
| 🎨 CSS | `--color-1: #…;` variables |
| { } JSON | Structured color data |
| 📄 TXT | HEX list, one per line |

You can also export the selected colors back to a **`.aco` file** with the **💾 Export .aco** button.

---

## 11. Mix history

- Found at the bottom of the **Mix colors** tab.
- Whenever you **copy** or **save** a mixed color, it's added to history automatically.
- **Click a history swatch** to copy it again.
- **✕** removes one color; **🗑 Clear history** removes all.
- History is **saved in your browser** (persists when you reopen the page).

---

## 12. Install as an app (PWA)

You can install the app on desktop and mobile:

| Platform | How |
|----------|-----|
| **Desktop** (Chrome/Edge) | Open the URL → **📲** button or the address-bar install icon → **Install** |
| **Android** (Chrome) | Open the URL → **⋮** menu → **Add to Home Screen** |
| **iPhone/iPad** (Safari) | Open the URL → **Share** → **Add to Home Screen** |

Once installed: it has its own icon, opens in a **standalone window** (no address bar), and works **offline**.

> **Requirement:** the app must be served over **HTTPS** (GitHub Pages / Netlify / Vercel). It cannot be installed from a local `file://`.

---

## 13. FAQ

**Q:** I opened a file but see no colors?
**A:** Check it's a valid `.aco` file. Some software exports ACO with a different structure.

**Q:** Is my data uploaded anywhere?
**A:** No. The app runs entirely in your browser — nothing is sent over the network.

**Q:** How does mixing work?
**A:** Colors are blended by ratio (weighted average) — like mixing paint. Drag a slider to make a color "heavier".

**Q:** How do I mix only part of an ACO file?
**A:** Click **📁 Open ACO file**, untick the colors you don't want, then click **Add colors to mix**.
