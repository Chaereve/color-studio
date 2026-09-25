# 🎨 Chaereve ColorLab — User Guide

A browser tool for viewing and editing Photoshop color swatches (`.aco`) and gradients (`.grd`).
**No install, nothing uploaded** — everything is processed locally on your machine.

---

## Contents

1. [Getting started](#1-getting-started)
2. [Language & font size](#2-language--font-size)
3. [Tab 1 — ACO colors](#3-tab-1--aco-colors)
4. [The color editor](#4-the-color-editor)
5. [Bulk adjust & shortcuts](#5-bulk-adjust--shortcuts)
6. [Tab 2 — .grd gradients](#6-tab-2--grd-gradients)
7. [Tab 3 — Mix colors](#7-tab-3--mix-colors)
8. [Tab 4 — Random colors](#8-tab-4--random-colors)
9. [Install as an app (PWA)](#9-install-as-an-app-pwa)
10. [FAQ](#10-faq)

---

## 1. Getting started

- Open `index.html` in any browser (Chrome, Edge, Firefox, Safari…).
- The app has **4 tabs**:
  - **ACO colors** — open, browse, search and edit `.aco` palettes.
  - **Gradients** — open and edit Photoshop `.grd` gradients.
  - **Mix** — blend several colors by ratio.
  - **Random** — generate random colors, one per member.
- The **⚙️** button (top right) opens settings. **VI / EN** switches language instantly.

---

## 2. Language & font size

- **VI / EN** in the top bar, or **⚙️ Settings → Language**: Tiếng Việt · English.
- **⚙️ Settings → Font size**: Small / Medium / Large.
- Choices are remembered. **Clear saved data** wipes the mix history and these options.

---

## 3. Tab 1 — ACO colors

### Opening a file
- **Drag and drop** an `.aco` (or `.grd`) file onto the panel, **or** click it to browse.
- Supports **ACO v1 & v2**, reading **color names** and RGB / HSB / CMYK / Lab / Grayscale spaces.
- Once loaded, the drop zone collapses to a compact bar — click it anytime to open another file.

### Browsing
- Each color is a card with an **index** (1, 2, 3…), a color chip, its name, HEX, RGB and the original color space.
- The index follows the **order inside the ACO file**.

### Copying
- **Click a card** to copy its code — HEX / RGB / HSL, chosen in the toolbar dropdown.
- **Copy all** copies every selected color in that same format.

### Selecting
- Click the **✓** in a card's corner to select / deselect it.
- The **Select** menu offers: select all · deselect all · invert selection.

### Search & sort
- The search box matches names, HEX or RGB.
- Sort by: original order · hue · lightness · saturation · name.

### Advanced search
Type these straight into the search box:
- `hue:0-60` — hue inside a range (red → yellow). `hue:>200`, `hue:<40`, `hue:120` also work.
- `sat:>50` — saturation above 50. Supports `<`, `>` and ranges like `20-80`.
- `light:40-80` — lightness inside a range.
- `similar:#FF0000` — the closest colors get a white outline.

### Editing the palette
- **Add** — pick a color in the square, then hit **Add**.
- **Rename** — the pencil button on a card.
- **Delete** — the trash button on a card.
- **Reorder** — drag and drop cards.
- **Right-click** a card for the quick menu (copy / details / rename / export .aco / delete).
- **Undo / Redo** — 60 steps.
- **Save .aco** — writes the whole palette back out to an `.aco` file (v2, with names).
- **Export .aco** — exports only the selected colors.

### Duplicates
The **Duplicates** menu has three options:
- **Mark / unmark** — outlines duplicate or near-identical colors in yellow.
- **Remove identical codes** — keeps one color per HEX.
- **Remove near-identical colors** — drops colors that sit very close to each other.

---

## 4. The color editor

One editor is used everywhere a color appears:

| Where | How to open |
|---|---|
| An ACO card | the **droplet** button on the card |
| A mixer chip | click the chip's **color square** |
| A random card | the **droplet** button in its corner |
| A `.grd` stop | click the stop's color square |
| Any color swatch | just click it |

Inside the editor:
- **Big square** — drag horizontally for saturation, vertically for value.
- **Hue slider** underneath.
- **HEX / R G B / H S L** fields you can type into.
- A live **old → new** preview with a suggested color name.
- **Revert** — back to the color you started with.
- **Add** — creates a new color instead of replacing one (where supported).
- An **eyedropper** button (Chromium) picks any color off the screen.

Every change is recorded in **Undo**.

---

## 5. Bulk adjust & shortcuts

- Select colors, then hit **Adjust** in the toolbar.
- Drag **Rotate hue / Saturation / Lightness** — the palette updates live as a preview.
- **Reset** returns the sliders to 0 · **Cancel** rolls everything back · **Apply** keeps the result (and records it in Undo).

| Key | Action |
|---|---|
| `Ctrl/Cmd + Z` | Undo |
| `Ctrl/Cmd + Shift + Z` or `Ctrl + Y` | Redo |
| `Ctrl/Cmd + A` | Select all colors |
| `Delete` / `Backspace` | Delete the selected colors |
| `Esc` | Close whatever is open |

---

## 6. Tab 2 — .grd gradients

- Drag and drop or click to open a `.grd` file (**v3 & v5**), both **solid** and **noise** forms.
- The gradient list is on the left — click one to edit it.
- For **solid** gradients: edit color stops (position, midpoint, color), transparency stops and smoothness.
- For **noise** gradients: edit seed, roughness, color limits and display options.
- **Add gradient** · **Delete gradient** · **Save .grd** writes a new file.
- You can also copy the CSS `linear-gradient`, export SVG, extract the colors to `.aco`, or send them to the ACO tab.

---

## 7. Tab 3 — Mix colors

- **Add colors** with the picker, or **Open ACO file** to pick from a whole palette.
- Dropping an `.aco` file onto the panel works too.
- **Equalize** splits the ratios evenly; drag a chip's slider to tune it individually.
- Click a chip's **color square** to retint it mid-mix.
- The result shows HEX / RGB / HSL — **click a row to copy it**.
- **Save to history** keeps the result; click a history entry to copy it again.
- **Load into ACO** sends the mix result to the ACO tab for further editing.

---

## 8. Tab 4 — Random colors

- Choose **Fully random** or **By color family** (8 families: red, orange, yellow, green, cyan, blue, purple, pink).
- Enter the **number of colors** (one per member) and tick **No duplicates** if needed.
- Hit **Random** to generate.
- Click a card to copy · the **droplet** button to hand-tune each one · **Load into ACO** to move them to the ACO tab.

---

## 9. Install as an app (PWA)

| Platform | How |
|---|---|
| **Windows / macOS / Linux** (Chrome, Edge) | Open the URL → the **install** icon in the address bar |
| **Android** (Chrome) | Menu ⋮ → **Install app** |
| **iPhone/iPad** (Safari) | Open the URL → **Share** → **Add to Home Screen** |

The app gets its own icon, opens in a standalone window and works **offline**.

---

## 10. FAQ

**Is my data uploaded anywhere?**
No. Everything is read and processed inside your browser.

**Which files can I open?**
`.aco` (v1 & v2) and `.grd` (v3 & v5).

**Can I edit colors and save them back to the original file format?**
Yes — after editing hit **Save .aco** and you'll download a new `.aco` file.

**How many undo steps?**
60 per opened file.

**Why don't I see the eyedropper button?**
It only appears on Chromium browsers (Chrome, Edge). Color editing works normally everywhere else.

**Where do I change the language?**
The **VI / EN** button in the top bar, or **⚙️ Settings → Language**.
