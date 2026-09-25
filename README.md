# 🎨 Chaereve ColorLab

<p align="center">
  <a href="https://github.com/chaereve/chaereve-colorlab/releases"><img alt="Download" src="https://img.shields.io/badge/Download-2ea043?style=for-the-badge"></a>
</p>

<p align="center">
  <a href="README.md"><img alt="English" src="https://img.shields.io/badge/English-22d3ee?style=for-the-badge"></a>&nbsp;
  <a href="README.vi.md"><img alt="Tiếng Việt" src="https://img.shields.io/badge/Ti%E1%BA%BFng%20Vi%E1%BB%87t-1a3fd6?style=for-the-badge"></a>&nbsp;
</p>

A tool to **view, mix, and export Photoshop (`.aco`) color palettes** — running entirely **in your browser**. No installation, no sign-up, no data upload.

> Everything is processed **100% locally** on your device.

**🌐 Bilingual UI:** Tiếng Việt · English — switch instantly from the header or in **⚙️ Settings**.

---

## ✨ Features

### 📁 View ACO
- Drag & drop (or click) a `.aco` file to open it.
- Supports **ACO v1 & v2**, reads **color names** and the RGB / HSB / CMYK / Lab / Grayscale color spaces.
- Each color shows an **index number**, name, HEX, RGB and its original color space.
- **Search** by name/HEX/RGB and **sort** by hue, lightness, saturation, or name.
- **Advanced search** — filter by ranges with `hue:0-60`, `sat:>50`, `light:40-80`, or find near-colors with `similar:#FF0000`.

### ✏️ Edit palette (in-place)
- **Rename** colors inline, **delete**, or **add** new colors — then **save back to .aco**.
- Full **undo / redo** (up to 60 steps).
- **Right-click** any swatch for a quick menu (copy / details / rename / export / delete).

### 🎛 Edit any color, anywhere
One shared **color editor** opens wherever a color appears — so you always get the same
picker instead of a different control on every screen:
- **Viewer** — the droplet button on every swatch card.
- **Mixer** — click the chip's color square to re-tint it and the mix updates instantly.
- **Random** — the droplet button on each generated card.
- **Harmony, Gradient, Contrast, Palette-from-image, .grd stops** — click any native
  color swatch (or the HEX label under a gradient stop) to open the editor.
- Inside the editor: **SV square + hue slider**, live **old → new** preview, and
  **HEX / RGB / HSL** fields you can type into. **Revert** jumps back to the original
  color; **Add** creates a new swatch instead of replacing one (where it applies).
- On Chromium browsers an **eyedropper** button picks any color off the screen.

### ⚡ Bulk adjust & shortcuts
- Select swatches, then **Điều chỉnh** to **rotate hue / saturation / lightness** across
  the whole selection with a live preview; **Reset** restores, **Cancel** rolls back.
- **Ctrl/Cmd + Z** undo · **Ctrl/Cmd + Shift + Z** (or **Ctrl + Y**) redo
- **Ctrl/Cmd + A** select all colors · **Delete / Backspace** delete the selected colors
- **Duplicate** menu: mark duplicates, remove identical codes, or remove near-identical colors.

### ➡ Send results to the Viewer
Every generator can hand its colors back to the main palette:
- **Random**, **Harmony**, **Palette-from-image**, **Gradient**, and the **mix result**
  all have a **Load into Viewer** button, so their colors become ordinary swatches you
  can keep editing.

### 📋 Copy
- Click a swatch to copy its code (**HEX / RGB / HSL** — selectable).
- **Copy all** as: HEX list, CSS variables, SCSS, JSON, RGB, **Tailwind config**, or **Styled Components**.

### 🎨 Mix colors (standalone — no ACO required)
- Add colors with the **color picker** or **open an ACO file** right in this tab.
- A selection grid lets you **exclude colors you don't want to mix** with one click.
- **Re-adjust your selection** without re-uploading the file.
- Ratios **auto-equalize** by color count; drag a slider to tweak each one.
- **Mix history** is saved automatically; click to copy again.

### 🎲 Random colors (per member)
- Generate 1–100 random colors for each "member", either fully random or within a chosen color family (red / orange / yellow / green / cyan / blue / purple / pink), with optional no-duplicate mode.

### 🛠 Design tools
Grouped under the **Create** and **Analyze** tabs:
- **Palette Generator** — complementary / analogous / triadic / split / tetradic.
- **Gradient Generator** — linear / radial / **conic** CSS gradient with copy-to-clipboard.
- **Image → Palette / Eyedropper** — click an image to pick a color, extract dominant colors, and **export them straight to .aco**.
- **Presets & Templates** — built-in Material Design, Tailwind, Brand Colors, Pastel and Earth Tones palettes.
- **Contrast Checker** — WCAG ratio with AA/AAA badges.
- **Accessibility Audit** — % of the palette passing AA against white/black text.
- **Palette Statistics** — average saturation/lightness and a hue-distribution chart.
- **Color Blindness Preview** — protanopia / deuteranopia / tritanopia / grayscale.
- **Color detail panel** — HEX / RGB / HSL / HSV / CMYK / Lab, luminance, contrast.
- **Duplicate detector** and **similar-color finder**.

### 📦 Batch processing
- Open **multiple .aco files** at once, then **merge** them into one palette (with optional dedup) or **export a merged .aco**.

### 🔗 Share palette
- Generate a **shareable link** (`?palette=...`) that encodes the current palette — anyone opening the link sees the same colors, no server needed.

### 📐 Gradient (.grd)
- Open Photoshop **gradient files** (`.grd`, **v3 & v5**) — solid and noise gradients.
- **Preview** each gradient, then **edit** color stops, transparency stops, midpoint, smoothness, and noise parameters (seed, roughness, min/max).
- **Add / remove gradients** and stops, then **save back to `.grd`**.
- Export a gradient as **CSS `linear-gradient`** or **SVG**, and **extract its colors to `.aco`** or straight into the Viewer.

### ⬇ Export
- **PNG / SVG / CSS / JSON / TXT** with layout, size, label and background options (including transparent).
- **ACO export** (v2, with color names) of your selected colors.

### 🌙 UI — Liquid Glass (dark only)
- **Liquid Glass** material: real backdrop blur with saturation, refractive rims and a specular top edge on glass surfaces.
- **Dark only** — the interface stays achromatic so your palette is the only thing in colour.
- **4 tab groups** instead of 7 scattered tabs: **View · Create · Analyze · Files**.
- **Stroke SVG icons** instead of emoji, a restrained type system, and motion limited to colour/opacity — no bouncing or glow.
- The ambient light behind the glass picks up the colours of the palette you have open.
- Responsive down to small phones.

### ⚙️ Settings
- **Language** — Tiếng Việt / English.
- **Font size** (small / medium / large).
- **Clear saved data** and an **About** box.

### 📲 Install as an app (PWA)
- Installable on **desktop (Windows/macOS/Linux)** and **mobile (Android/iOS)**.
- Has its own icon, opens in a standalone window, and works **offline**.

### 🖥 Desktop version (Windows)
- Packaged as a **native Windows desktop app** using Electron — see the `electron-app/` folder.
- Build a **Windows** installer: `.exe` (NSIS installer + portable).
- The app logo has **rounded-square corners**, like modern apps.

---

## 🚀 Usage

### On desktop / mobile
Just open `index.html` in any browser (double-click it), or visit the deployed URL.

### Quick flow
1. Open the **📁 View ACO** tab → drag & drop a `.aco` file.
2. Click a color to copy it, or tick several colors to export them.
3. Open the **🎨 Mix colors** tab → add colors → see the mix result instantly.
4. Click **⬇ Export image & data** to download the palette.
5. Open the **📐 Gradient** tab → drop a `.grd` file to view and edit Photoshop gradients.
6. Open **⚙️ Settings** (or use **VI / EN** in the header) to switch language and font size.

---

## 🌐 Languages (2)

Switch with the **VI / EN** control in the header, or via **⚙️ Settings → Language**: Tiếng Việt · English. The whole interface switches instantly and your choice is remembered across sessions.

| Language | README | User Guide |
|----------|--------|------------|
| 🇬🇧 English | [README.md](README.md) | [USER_GUIDE.md](USER_GUIDE.md) |
| 🇻🇳 Tiếng Việt | [README.vi.md](README.vi.md) | [USER_GUIDE.vi.md](USER_GUIDE.vi.md) |

---

## 📲 Install as an app (PWA)

Once the app is deployed (over HTTPS), you can install it as a real app:

| Platform | How |
|----------|-----|
| **Desktop** (Chrome/Edge) | Open the URL → click the **📲** button (top-right) or the install icon in the address bar → **Install** |
| **Android** (Chrome) | Open the URL → **⋮** menu → **Add to Home Screen** |
| **iPhone/iPad** (Safari) | Open the URL → **Share** button → **Add to Home Screen** |

> **Important:** PWAs must be served over **HTTPS** (GitHub Pages, Netlify and Vercel all do this). You cannot install when opening a `file://` directly.

---

## ❓ FAQ

**Is my data uploaded anywhere?**
No. Everything runs in your browser — nothing is sent over the network.

**The file opens but no colors appear?**
Check that it's a valid `.aco` file. Some apps export ACO with a non-standard structure.

**How does color mixing work?**
The app blends colors by ratio (weighted average) — like mixing paint. Drag a slider to make a color "heavier".

**How do I mix only some colors from a file?**
Open the ACO in the **Mix colors** tab → click to deselect the colors you don't want → click **Add colors to mix**.

---

## 📚 Guides

User guide:
- 🇬🇧 [USER_GUIDE.md](USER_GUIDE.md) · 🇻🇳 [USER_GUIDE.vi.md](USER_GUIDE.vi.md)

---

## 📄 License

Free to use for personal and commercial work.
