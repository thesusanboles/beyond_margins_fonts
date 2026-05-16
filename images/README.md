# Beyond Margins — site images to host on GitHub

All the images needed for both the **Services page** and **Capacity
Escape Hatch** page, plus one bonus pattern (`grain-on-green.png`) saved
for future use. Drop these 8 files into the root of your
`thesusanboles/beyond_margins_fonts` GitHub repo — same place the
.woff2 files live — and jsDelivr will serve each at:

```
https://cdn.jsdelivr.net/gh/thesusanboles/beyond_margins_fonts@main/<filename>.png
```

Once they're up, send me back the base URL and I'll stage the code
injection update.

## File inventory

### Decorative patterns (used as CSS backgrounds)

| File | Used on |
|---|---|
| `topography.png` | Capacity Escape Hatch hero + final CTA · Services-page good-fit + BusinessOS |
| `halftone-black.png` | Capacity Escape Hatch principles · Services-page philosophy + service-footer + footer |
| `mountains-green.png` | Services-page hero pattern disc |
| `mountains-green-soft.png` | Services-page final CTA |
| `grain-on-green.png` | *(none currently — included for future use)* |

### Page-specific imagery (used as `<img src>`)

| File | Used on |
|---|---|
| `banner-wheel.png` | Capacity Escape Hatch hero — the wheel-wordmark banner |
| `susan-photo.png` | Capacity Escape Hatch About section — large halftone portrait collage |
| `susan-avatar.png` | Capacity Escape Hatch email preview card — small green-blob bust |

## What I'll do once you send me the URL

1. **Update `code-injection-current.html`** — flip 4 `--bm-pattern-*`
   CSS variables from `none` to the live `url(...)`. Staged as
   `code-injection-next.html` so you can paste it into Ghost
   (Settings → Code Injection → Site Header) in one go.
2. **Note the image URLs** in the project README so they're easy to
   reference when we deploy the Capacity Escape Hatch page HTML
   (which references `banner-wheel.png`, `susan-photo.png`, and
   `susan-avatar.png` directly — those URLs need to be swapped into
   the page-html.html before pasting).
