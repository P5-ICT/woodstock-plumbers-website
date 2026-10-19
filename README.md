# Woodstock Plumbers 24/7 — Website

A single-page website concept for Woodstock Plumbers 24/7, 1 Essex St, Woodstock, Cape Town.

## Run it locally

No build step, no dependencies — plain HTML/CSS/JS.

**Easiest way:** double-click `index.html`.

**Or run a local server:**

```bash
cd woodstock-plumbers-website
python3 -m http.server 8000
# then open http://localhost:8000
```

```bash
npx serve .
```

## Files

- `index.html` — the whole site
- `assets/` — real job photos used in the "Recent Work" section, split into two groups:
  - Installations: `valve-manifold.png`, `ceiling-pipework-tanks.png`, `geyser-install.png`,
    `outdoor-geyser-install.png`, `outdoor-meter-box.png`
  - Bathroom renovations: `before-strip-out.png` (before), `bathroom-double-vanity-mirrors.png` (after),
    plus `bathroom-fittings.png`, `bathroom-toilet-window.png`, `bathroom-shower-vanity.png`,
    `bathroom-walkin-shower.png`, `bathroom-freestanding-tub.png`

## Notes on the source data

- Contact details (address, phone, hours) came from the business's Google listing and were
  consistent across sources this time — no conflicting info to flag.
- The listing showed two different rating/review totals (4.9★/37 reviews on one card, 4.6★/25
  on another), which usually means there's more than one Google Business listing for the same
  company. Rather than guess which is right, the site doesn't display an aggregate star rating —
  just real testimonials, which is the safer call either way.
- Testimonials are paraphrased from genuine positive Google reviews, attributed by first name +
  last initial only. As with any business, there were also negative reviews; a marketing site
  reasonably leads with the positive ones (same as any business does), but it's worth being aware
  the reviews were mixed if you're pitching this as a portfolio example.

## Known limitations (before this could go live for a real client)

- Booking form is front-end only — no backend, no emergency dispatch. For a 24/7 emergency
  business this matters more than most: real intake would need to route to an actual on-call
  phone/SMS system, not just an email inbox, or people in genuine emergencies could be left
  waiting on a form nobody's watching.
- Map is a placeholder box, not a live embed (needs a Maps API key).
- No hosting/domain yet — this is just the code.
