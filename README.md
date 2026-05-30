# 🎀 Birthday Website for XYZ

A gorgeous Apple-style scroll birthday website with password lock, pink animations, and scroll-reveal effects.

---
   **`https://YOUR-USERNAME.github.io/birthday-xyz`**
---

## ✏️ How to Customize

Open `index.html` and scroll to the `CONFIG` block at the top of `<script>`:

```javascript
const CONFIG = {
  name:     "XYZ",      // ← Change to her real name
  password: "1430",     // ← Change the secret password

  pinSlides: [
    { img: "images/photo1.jpg", heading: "Her Smile", body: "..." },
    // add real image paths here
  ],

  pickupLines: [ ... ],   // edit cute lines
  reasons:     [ ... ],   // edit reasons she's great
  memories:    [ ... ],   // add memory photos
};
```

---

## 🖼️ Adding Her Photos

### Option A — GitHub (recommended)
1. Create a folder called `images/` in your repo
2. Upload her photos there (e.g. `photo1.jpg`, `photo2.jpg`)
3. In CONFIG, set: `img: "images/photo1.jpg"`

### Option B — Google Drive / Imgur
- Upload to Imgur → copy direct link → paste as `img: "https://i.imgur.com/xxx.jpg"`

### Where to add photos:
| Config key | What it affects |
|---|---|
| `pinSlides[i].img` | The big Apple-style scroll section (4 slides) |
| `memories[i].img` | The masonry photo wall at the bottom |
| Reveal sections | Find `img-placeholder` divs in HTML, replace with `<img src="...">` |

---

## 🎨 Change Colors
All colors are CSS variables in `:root` — just change the hex values:
```css
--pink-deep:  #c9517a;   /* dark pink */
--pink-main:  #e8789a;   /* main pink */
--pink-soft:  #f4a7be;   /* soft pink */
--pink-blush: #fce4ec;   /* very light */
```

---

## 🔒 Password
Default password is `1430`. Change it in CONFIG:
```javascript
password: "1430",   // ← change this
```
The input shows pink hearts (♥) as you type — turns red if wrong, unlocks with animation if correct.

---

Made with 💗 By Moin Shadab — one file, zero dependencies, deploys free on GitHub Pages.
