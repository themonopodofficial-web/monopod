# MONOPOD — Website Project

A cinematic black & white portfolio website for Monkive Visual Production Studio.

---

## 📁 Folder Structure

```
monopod/
├── index.html                  ← The website (open this in a browser)
├── README.md                   ← This file
└── images/
    ├── hero/                   ← 3 background images for the homepage hero
    ├── music-video/            ← Photos for Music Video project
    ├── photoshoot/             ← Photos for Photoshoot project
    ├── usurey/                 ← Photos for Usurey - Music Video Color Grade
    └── wtf-short-film/         ← Photos for WTF - Short Film
```

---

## 🖼️ How to Add Your Photos

### Step 1 — Copy photos into the right folder

Download your photos from Google Drive and put them in the matching folder:

| Project | Folder |
|---|---|
| Music Video | `images/music-video/` |
| Photoshoot | `images/photoshoot/` |
| Usurey - Color Grade | `images/usurey/` |
| WTF - Short Film | `images/wtf-short-film/` |
| Hero background (pick 3) | `images/hero/` |

**Supported formats:** `.jpg` `.jpeg` `.png` `.webp`

> 💡 Tip: Rename your files simply — e.g. `01.jpg`, `02.jpg`, `03.jpg`

---

### Step 2 — Tell the website about your files

Open `index.html` in any text editor (Notepad, VS Code, etc.)

Find this section near the bottom (~line 280):

```javascript
const IMAGES = {
  "music-video": [
    // "photo1.jpg",
  ],
```

Remove the `//` and fill in your actual filenames. Example:

```javascript
const IMAGES = {
  "music-video": [
    "01.jpg",
    "02.jpg",
    "03.jpg",
    "04.jpg",
  ],
  "photoshoot": [
    "01.jpg",
    "02.jpg",
    "05.jpg",
  ],
  "usurey": [
    "cover.jpg",
    "behind-scenes.jpg",
  ],
  "wtf-short-film": [
    "still1.jpg",
    "still2.jpg",
    "still3.jpg",
  ],
  "hero": [
    "music-video/01.jpg",
    "photoshoot/01.jpg",
    "wtf-short-film/still1.jpg",
  ]
};
```

Save the file. Open `index.html` in your browser — photos appear immediately.

---

## 🚀 How to Host FREE on GitHub Pages

### First time setup:

1. Go to [github.com](https://github.com) and create a free account
2. Click **New Repository**
3. Name it: `monopod` (or `yourusername.github.io` for a root URL)
4. Set to **Public**, click **Create repository**

### Upload your files:

**Option A — Drag & Drop (easiest):**
1. Open your repo on GitHub
2. Click **Add file → Upload files**
3. Drag the entire `monopod` folder contents (index.html + images/)
4. Click **Commit changes**

**Option B — GitHub Desktop app:**
1. Download [GitHub Desktop](https://desktop.github.com)
2. Clone your repo
3. Copy all files into the cloned folder
4. Commit & Push

### Enable GitHub Pages:
1. Go to your repo → **Settings** → **Pages**
2. Under Source, select **main** branch → **/ (root)**
3. Click **Save**
4. Your site is live at: `https://yourusername.github.io/monopod`

---

## ✏️ Customisation

All editable content is in `index.html`:

| What | Where to find it |
|---|---|
| Studio name | Search `MONOPOD` |
| About text | Search `We frame the world` |
| Project names & years | Search `proj-name` |
| Social links | Search `soc-row` |
| Contact email | Add `action="mailto:you@email.com"` to the form |
| Stats (4 projects, etc.) | Search `stat-num` |

---

## 📷 Photo Tips

- **Best dimensions:** 1920×1080px or wider for landscape, 1080×1350px for portrait
- **File size:** Keep each image under 500KB for fast loading (use [squoosh.app](https://squoosh.app) to compress)
- The site applies a **grayscale + contrast filter** automatically — color photos will look great in B&W
- Each project shows a **slideshow** if you add multiple images — arrows and dots appear on hover

---

Built with Bootstrap 5 · Unbounded + Lora + DM Mono fonts · No frameworks required
