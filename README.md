# The Cushion Store / Cloud Dry — Web Catalog
Self-contained static catalogs for shoppers and specifiers: a **Technical Story** and an interactive **OEM Fit Tool**. Vanilla HTML, CSS, and JavaScript. No build step. Home: Milwaukee, WI.

## Open locally

Double-click `index.html`, or from this folder:

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

`file://` is supported. Relative paths only; no CDN fonts or runtime dependencies.

To serve over HTTP (optional):

```bash
python3 -m http.server 47281
```

Then open `http://127.0.0.1:47281/`.

Drop the folder on any static host (GitHub Pages, Netlify, S3, nginx). No server-side logic.

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Cloud Dry Technical Story — batting displacement, core matrix, textiles/COM, aesthetics, CNC |
| `fit.html` | OEM Fit Tool — search, brand, and type filters across 94 drop-in SKUs |
| `brands.html` | Top-20 brand directory — 12 live + 8 research-only fitment cards |
| `brand-directory-data.js` | `window.TCS_BRAND_DIRECTORY` — Spec shortlist for directory cards |
| `sources.html` | Quiet performance-basis links for engineered ILD / ASTM targets |
| `styles.css` | Architectural coastal design system (linen, slate, navy + light blue) |
| `fit-data.js` | `window.TCS_SKUS` — 94 records from the OEM replacement master |
| `assets/cloud-dry-hero.png` | Lifestyle terrace hero |
| `assets/cloud-dry-detail.png` | Boxed cushion welt detail |

## Fit Tool

Search OEM code, model, or name. Filter by brand family and type (dining, deep seat, chaise, ottoman, pillow, bench, specialty). Each card shows Model, OEM line, configuration, exact dimensions, Cloud Dry core / ILD, and COM yield at 54".

Example: **Ebel 6001** → `TCS-6001`, dining 20×18×3, Cloud Dry reticulated ILD 35–45, COM 1.0 yd.

## Naming

Customer-facing brand is **The Cushion Store** only. Product language uses **Cloud Dry** for reticulated outdoor foam. Do not brand the product as Dry-Fast. Model codes use the `TCS-` prefix.

ILD and ASTM values are engineered targets pending laboratory confirmation. Dimensions and COM on listed SKUs are customer-brief authoritative.

## Prestige photography

`assets/prestige/` holds the coastal navy prestige set (01–32). Each file is used at most once across `index.html` + `fit.html` + `sources.html`.

### Technical Story (`index.html`) — photos 01–08 only

| File | Placement |
| --- | --- |
| `01-twilight-terrace.png` | Hero background |
| `02-poolside-chaise.png` | Why-replace-batting figure |
| `03-dining-terrace.png` | Cloud Dry matrix accent |
| `04-marina-lounge.png` | Textiles & COM figure |
| `05-morning-porch.png` | Beauty checklist accent |
| `06-garden-sectional.png` | Aesthetics primary figure |
| `07-evening-glow-lounge.png` | CNC craft pair (left) |
| `08-rain-ready-terrace.png` | CNC craft pair (right) |

### OEM Fit Configurator (`fit.html`) — photos 09–32 only

| File | Placement |
| --- | --- |
| `09-courtyard-dappled.png` | Hero photo strip |
| `10-lakeside-lounge.png` | Hero photo strip |
| `11-screened-porch.png` | Hero photo strip |
| `12-rooftop-bluehour.png` | Hero photo strip |
| `13-ottoman.png` | Hero photo strip |
| `14-lumbar.png` | Hero photo strip |
| `15-dining-pad.png` | Builder step 2 illustration |
| `16-sectional-corner.png` | Hero photo strip |
| `17-boxed-seat-hero.png` | Hero photo strip |
| `18-welt-detail.png` | Catalog header accent |
| `19-deep-seat-stack.png` | Hero photo strip |
| `20-chaise-pad.png` | Hero photo strip |
| `21-boxing-corner.png` | Catalog header accent |
| `22-foam-cutaway.png` | Hero photo strip (solid cushion still — no foam pore imagery) |
| `23-fabric-bolt.png` | Builder step 3 illustration |
| `24-cnc-core.png` | Hero photo strip (solid cushion still — no foam pore imagery) |
| `25-guest-ready.png` | Builder step 4 illustration |
| `26-shade-chaise.png` | Hero photo strip |
| `27-intimate-dining.png` | Hero photo strip |
| `28-ties-stitch.png` | Catalog header accent |
| `29-contrast-welt.png` | Catalog header accent |
| `30-lakefront-morning.png` | Hero photo strip |
| `31-pillow-pair.png` | Hero photo strip |
| `32-dusk-hospitality.png` | Builder step 1 illustration |

`sources.html` does not use prestige photos. Do not reuse 01–08 on `fit.html` or 09–32 on `index.html`.


## Christian lock (2026-09-22)

1. **Eight research brands approved** as fitment-ID directory cards only (Tropitone, Brown Jordan, Woodard, Summer Classics, Homecrest, Kingsley Bate, Castelle, Frontgate) — no fake SKUs until dims/COM brief.
2. **Classic dim freezes** — drop-in claims frozen until a real re-brief: `TCS-C-31D`, `TCS-C-55W4`, `TCS-C-5DS010`. Cards remain visible with freeze copy; builder selection is disabled. Research: `/workspace/tcs-cloud-dry-research/classic-cushions-deep-dive.md`.


## Imagery note

Foam pore / cutaway close-ups are archived under `assets/prestige/_trypophobia_archive/`. Live pages use solid cushion and lifestyle stills only.
