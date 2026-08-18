# Mike Dodds - independent website (v1)

Static one-page site. Open `index.html` in any browser. No build step, no dependencies to install.

```
Website Jul 2026/
├── index.html      ← the whole site (HTML + CSS + a few lines of JS)
└── assets/         ← 8 images, web-sized
```

## Design direction - "Ground Truth"

The visual language is **land survey**: aerial photography annotated with surveyor's marks (corner ticks, boundary frame, crosshair) that draw themselves on load. Palette is bush-shadow green, limewash chalk, vineyard green and brass - deliberately *not* the cream-and-serif look every estate agent site uses. Type: Archivo (wide, signage-like) for headlines, Source Serif 4 for reading, IBM Plex Mono for survey labels.

Positioning throughout: **the man, not the brand.** Owner's perspective, answers his own phone, knows two markets properly.

**Scope (Aug 2026 update):** commercial **and** agricultural specialist working **across South Africa**, based in the Western Cape. Regional history (Winelands, Lowveld) is kept as credibility, not as the limit of where he works.

## What's real vs. what needs confirming

| Item | Status |
|---|---|
| All bio copy, career history, regions, family details | From Mike's own bio document |
| Mobile 082 906 7004 (call + WhatsApp links) | From his own published advert - **verify before launch** |
| Photography | **No former-brokerage properties.** Hero, portrait and desk shots supplied by Nathi (Aug 2026); agricultural + commercial cards generated generically; bush/family photos are Mike's own |
| **Email `mike@mikedodds.co.za`** | **PLACEHOLDER - domain not registered.** Replace in `index.html` (marked with a TODO comment) |
| No agency branding anywhere | Every image that showed a property he marketed under the previous brokerage has been retired to `_retired assets/`; footer carries an explicit non-affiliation statement |

## Deliberate omissions

- **No listings section.** Nothing on the site claims a sale, a price or a testimonial - everything stated is verifiable from his bio. Add real listings/testimonials once approved.
- **No new-company mention.** The new brokerage appears nowhere, per the brief.
- **Retired images** live in `_retired assets/` - not deleted, but not referenced by the site.
- Photos of properties are used as *illustrations of property type*, with no price or status attached.

## To put it live

1. Register a domain (`mikedodds.co.za` reads best and matches the placeholder email).
2. Drag this folder into **Netlify Drop** (netlify.com/drop) or Cloudflare Pages - free, instant, HTTPS included.
3. Point the domain at it, then swap the email address in `index.html`.

## Easy edits

Everything lives in one file. Colours are CSS variables at the top of the `<style>` block. Section copy is plain HTML - search for the visible text and change it. To swap a photo, drop a replacement into `assets/` with the same filename.

## Next version ideas

- Listings grid fed by a simple JSON file
- Enquiry form (Netlify Forms - free, no backend)
- Afrikaans language toggle for Winelands farming clients
- A short Remotion intro video for the hero, using the same brand system as the vVvone ads
