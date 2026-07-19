# Bubba's Coffee — Shopify Theme

Built from scratch for Bubba's Coffee (Koh Phangan), a tropical hospitality
and coffee/lifestyle brand. Structured per Shopify Online Store 2.0
conventions and targeting 2026 Core Web Vitals thresholds (LCP < 2.5s,
INP < 200ms, CLS < 0.1).

## Brand tokens (from Bubbas_Brand_Guidelines.pdf)

| Token | Hex | Use |
|---|---|---|
| Jungle Green | `#222A13` | Primary dark / header bg |
| Roast Brown | `#301C12` | Secondary dark / footer bg |
| Island Gold | `#EED483` | Primary light / accent, CTAs |
| Faded Cream | `#FEF2C6` | Secondary light / page background |

**Typography:** Allora (logo/headings), Alosta (subheadings/CTA),
Raleway (body copy, wide tracking). Allora/Alosta are not standard
Shopify font-picker fonts — upload the licensed font files under
Settings → Theme → Fonts (or as custom assets) to get an exact match;
Raleway is currently mapped as the fallback for all three.

All values live in `config/settings_schema.json` / `settings_data.json`
so they're editable in the Theme Editor without touching code.

## Structure

```
layout/theme.liquid        Base HTML shell, loads CSS vars from settings
sections/header.liquid     Site header + nav
sections/footer.liquid     Site footer (hours, socials)
sections/hero.liquid       Homepage hero (reusable on any page)
templates/index.json       Homepage template
snippets/meta-tags.liquid  SEO + LocalBusiness structured data
assets/base.css            Core styles (mobile-first)
assets/global.js           Minimal JS (kept light for INP)
```

## Next build steps

- [ ] Upload logo assets (primary wordmark, stacked, brand motif) via Theme Editor
- [ ] Upload/license Allora + Alosta font files for exact type match
- [ ] Build product/collection templates (coffee catalog)
- [ ] Build "Our Story" / lifestyle content sections
- [ ] Add Product structured data on product template
- [ ] Connect this repo/branch to an unpublished theme in Shopify Admin
