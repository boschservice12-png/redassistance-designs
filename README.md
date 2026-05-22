# RedAssistance — Design Archive

Privát-építésű, publikus design archívum a RedAssistance ecosystem-hez. Self-contained HTML landing oldalak, kampány-design-ok, modul-bemutatók. Élesítés GitHub Pages-en keresztül.

**Élő archívum:** https://boschservice12-png.github.io/redassistance-designs/
**Katalógus:** [`_index.md`](_index.md)

## Mappa-struktúra

```
.
├── README.md              ← ez a fájl
├── _index.md              ← élő design-ok katalógusa
├── live/                  ← production-ready design-ok (Pages-deployolva)
│   └── sezonier-roti/
│       ├── index.html     ← self-contained landing page
│       ├── meta.yaml      ← gépi metadata
│       └── README.md      ← belső dokumentáció
├── draft/                 ← munka-verziók (nincs auto-deploy elvárás)
├── test/                  ← kísérletek, A/B teszt változatok
├── archive/               ← deprecated, történeti
└── assets/                ← közös brand tokenek
    ├── colors_and_type.css
    └── README.md
```

## Workflow

1. Új design HTML-t bemásolsz Claude-nak
2. Claude self-contained-re alakítja (inline CSS + SVG, no external file deps)
3. Commit a `live/<slug>/index.html` útvonalra a `main` branch-en
4. GitHub Pages 60–90 mp alatt automatikusan deploy-olja
5. Az élő URL: `https://boschservice12-png.github.io/redassistance-designs/live/<slug>/`

## Brand szabályok

- **Primary red:** `#E11D2E`
- **Font:** Geist (sans), Geist Mono (mono) — Google Fonts CDN-ről
- **Self-contained kötelező:** minden `live/*/index.html`-nek önállóan kell működnie (inline CSS + inline SVG), hogy ne legyen relatív-útvonalas törött asset a Pages deploy után.

## Fájlnév-konvenció

- `live/<slug>/index.html` — Pages-friendly slash-routing (élő verzió)
- `archive/YYYY-MM-DD_<slug>_vN.html` — verzió-követéshez deprecated design-oknál

## Licenc

Belső használat — minden jog fenntartva, SC Szkaliczki Service SRL.
