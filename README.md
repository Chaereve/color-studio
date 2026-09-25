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

### 📁 1. View & edit ACO colors
- Drag-and-drop (or click) to open an `.aco` file. Supports **ACO v1 & v2**, reading **color names** and RGB / HSB / CMYK / Lab / Grayscale spaces.
- Every color shows its index, name, HEX, RGB and original color space.
- **Search** by name/HEX/RGB · **sort** by hue / lightness / saturation / name.
- Advanced filters: `hue:0-60` · `sat:>50` · `light:40-80` · `similar:#FF0000`.
- **Add / delete / rename / drag-to-reorder** · full **undo / redo** (60 steps) · **save back to .aco**.
- **Right-click** a swatch for the quick menu.

### 🎛 2. One color editor, everywhere
- A **droplet button** on every ACO swatch, every random card, and every mixer chip's color square.
- Every other color swatch (.grd stops, base colors…) opens that same editor.
- **SV square + hue slider**, live **old → new** preview, typeable **HEX / RGB / HSL**.
- **Revert** jumps back to the original color · **Add** creates a new swatch instead of replacing one.
- An **eyedropper** button (Chromium) picks any color off the screen.
- Every change goes through **undo**.

### ⚡ 3. Bulk adjust & shortcuts
- Select colors, hit **Adjust** to **rotate hue / saturation / lightness** with a live preview; **Reset** restores, **Cancel** rolls back.
- **Ctrl/Cmd + Z** undo · **Ctrl/Cmd + Shift + Z** (or **Ctrl + Y**) redo
- **Ctrl/Cmd + A** select all · **Delete / Backspace** delete the selected colors
- **Duplicates** menu: mark · remove identical codes · remove near-identical colors.

### 🌈 4. .grd gradients
- Open Photoshop gradient files (`.grd` **v3 & v5**) — solid and noise forms.
- Edit color stops, transparency stops, midpoints, smoothness, noise parameters; add / remove gradients and stops.
- **Save back to `.grd`** · copy CSS · export SVG · extract colors to `.aco` · send to the ACO tab.

### 🎨 5. Mix colors
- Add colors with the color picker or **open an ACO file** right in the tab; a selection grid lets you exclude colors.
- Ratios auto-equalize; drag a slider to tweak each one; **equalize** everything in one click.
- Click the result's **HEX / RGB / HSL** row to copy · **save to history** · **send to the ACO tab**.
- Click a chip's color square to retint it mid-mix.

### 🎲 6. Random colors
- Generate 1–100 colors, one per "member", fully random or within a color family (8 families), with an optional no-duplicate mode.
- Click to copy · droplet button to hand-tune each one · **send to the ACO tab**.

### 🌙 UI — Liquid Glass (dark only)
- **Liquid Glass**: real backdrop blur with saturation, refractive rims and a top highlight on glass surfaces.
- **Dark only** — an almost achromatic UI so your colors are the only colorful thing.
- **4 tabs: ACO colors · .grd gradients · Mix · Random.**
- Stroke **SVG icons** instead of emoji, clear type hierarchy, motion limited to color/opacity — no bounce, no glow.
- The ambient light behind the glass is tinted by the palette you have open · works well on small screens.

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
1. Open the **ACO colors** tab → drag & drop a `.aco` file.
2. Click a card to copy · the droplet to edit · the pencil to rename.
3. Select several colors, then hit **Adjust** to shift hue / lightness in bulk.
4. Hit **Save .aco** to download the edited palette.
5. Open the **Gradients** tab → drop a `.grd` file to view and edit Photoshop gradients.
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
