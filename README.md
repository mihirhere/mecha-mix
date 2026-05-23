# Mecha-Mix — Website

The project site for **Mecha-Mix**, the NYU Tandon Senior Design capstone by *The Alchemists* (Jason He · Anthony Huanca · Sahil Krishnani · Youssef Mikhaiil · Mihir Pabby).

```
.
├── index.html              # main scrolling landing page
├── engineering.html        # technical deep-dive with KaTeX math
├── gallery.html            # photographs from the showcase
├── report.html             # the full design report, embedded inline
├── README.md               # this file
├── .nojekyll               # tells GitHub Pages NOT to run Jekyll
├── assets/                 # logo, mark, CAD renders, CFD
│   └── showcase/           # 19 showcase photographs
└── documents/              # report PDF + poster PDF
```

---

## How to host this on GitHub Pages — step by step

### 1. Make a GitHub account (skip if you have one)
Go to **[github.com](https://github.com)** → **Sign up**.

### 2. Create a new repository
1. Top-right → **+** → **New repository**.
2. **Repository name:** `mecha-mix` (this becomes part of your URL).
3. **Public** (must be public for free GitHub Pages).
4. **Do NOT** check "Add a README" — we already have one.
5. Click **Create repository**.

### 3. Upload the site files
1. On the new empty repo page, click the **"uploading an existing file"** link.
2. Open the `mecha-mix-website` folder on your computer.
3. **Select EVERYTHING inside the folder** (Cmd/Ctrl+A) — HTML files, `assets/`, `documents/`, `README.md`, and the hidden `.nojekyll`.
   - On Mac, press `Cmd + Shift + .` in Finder to show hidden files like `.nojekyll`.
   - On Windows, View → check **Hidden items** in File Explorer.
4. Drag everything into the GitHub upload area. Wait for all files to finish uploading.
5. Scroll down → commit message like *"Initial site"* → **Commit changes**.

### 4. Turn on GitHub Pages
1. In your repo, click the **Settings** tab.
2. Left sidebar → **Pages**.
3. Source: **Deploy from a branch**.
4. Branch: `main` · folder `/ (root)` → **Save**.
5. Wait ~1–2 minutes. Refresh the Settings → Pages screen. The live URL appears at the top:
   > Your site is live at `https://<your-username>.github.io/mecha-mix/`

Open it. Done.

### 5. Custom domain (optional)
1. Settings → Pages → **Custom domain** → enter your domain → Save.
2. With your domain registrar, add a `CNAME` record pointing to `<your-username>.github.io`.
3. After ~10 minutes for DNS, check "Enforce HTTPS".

---

## Editing the site

### Add or replace a showcase photo
Photos live in `assets/showcase/`. Each is referenced by name in `index.html` and `gallery.html`. To swap one:

1. Upload your new photo to `assets/showcase/` (JPG, ideally ~1600 px wide).
2. In `gallery.html` or `index.html`, search for the existing filename (e.g. `team-with-poster.jpg`) and replace with your new one.

### Update team roles
Open `index.html`, search for `roster`. The `<div class="roster">` block has each team member's name + role. Edit freely.

### Make text changes
All copy is in plain HTML — open any `.html` file in a text editor and edit. Save, commit, push. Live in ~30 seconds.

### Local preview (no install needed)
Just double-click `index.html` to open it in your browser. For full PDF preview and proper inter-page links, run a local server: open Terminal in the folder and run `python3 -m http.server`, then visit `http://localhost:8000`.

---

## Design notes

- **Type:** [Fraunces](https://fonts.google.com/specimen/Fraunces) (variable serif headlines), [DM Sans](https://fonts.google.com/specimen/DM+Sans) (body), [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (technical callouts). All Google Fonts.
- **Math:** Engineering equations rendered with [KaTeX](https://katex.org/) for proper typography.
- **Colors:** Pulled from the Mecha-Mix brand — deep navy `#0B1422`, cream `#F1E6CE`, orange `#E08438`.
- **No build step.** Plain HTML/CSS/JS. Edit any file and refresh.
- **PDF embed:** `report.html` uses an `<iframe>` to embed the full design report inline. Modern browsers render it via their built-in PDF viewer; older browsers fall back to a download link.

---

## Credits

- **Project:** Mecha-Mix — The Alchemists, NYU Tandon ME-UY 4113, 2025–26.
- **Photography:** Senior Design Showcase event photography (May 5, 2026).
- **Site:** Generated with Claude (Anthropic).
- **Fonts:** Fraunces (Undercase Type), DM Sans (Indian Type Foundry), JetBrains Mono (JetBrains) — SIL OFL.
