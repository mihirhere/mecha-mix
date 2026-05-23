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
