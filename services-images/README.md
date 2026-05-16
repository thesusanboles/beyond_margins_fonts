# Services page — image bundle

Six images referenced by the Ghost section cards and the page CSS. Upload this folder structure to GitHub **exactly as-is** — the folder layout matches the paths in the HTML/CSS.

```
services-images/
├── photo-graphic-2.png       ← hero portrait
├── divider-squiggle.png      ← squiggle in the good-fit section
└── patterns/
    ├── halftone-black.png    ← philosophy / dark sections
    ├── mountains-green.png   ← hero pattern circle
    ├── mountains-green-soft.png  ← final-CTA texture
    └── topography.png        ← good-fit + businessOS pattern
```

## After upload

Get the **raw** base URL for the folder on GitHub:

- Repo file URL looks like: `https://github.com/<user>/<repo>/blob/main/services-images/photo-graphic-2.png`
- Raw URL is: `https://raw.githubusercontent.com/<user>/<repo>/main/services-images/photo-graphic-2.png`
- So your `ASSETS_BASE` =  `https://raw.githubusercontent.com/<user>/<repo>/main/services-images`

Tell me that URL and I'll do the find-and-replace across `bm-services-page.css` and the 8 HTML cards.

> **Tip:** For Ghost specifically, **jsDelivr** is a friendlier CDN than `raw.githubusercontent.com` (proper cache headers, no rate-limit, served as `image/*`). Same path, different host:
> `https://cdn.jsdelivr.net/gh/<user>/<repo>@main/services-images`
>
> This is the same pattern your existing brand-fonts host uses (`cdn.jsdelivr.net/gh/thesusanboles/beyond_margins_fonts`), so it'll be consistent.
