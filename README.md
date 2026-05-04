# Profit First Calculator

A no-build, single-file web tool that walks a small business owner through a short questionnaire and produces their starting Profit First allocations.

Built originally for a friend launching a video production company, written generically so it can serve as a Five One Nine Marketing lead magnet.

## What it does

- 6-step mobile-first wizard
- Plain-English explanations of every term, with on-tap tooltips
- Computes recommended Profit / Owner's Comp / Tax / OpEx percentages based on:
  - Full-time vs. side hustle
  - Entity type (sole prop / LLC / S-corp)
  - Projected year-one revenue
  - Per-project sub costs
  - Debt status
  - Personal monthly cost of living
- Adjustable sliders on the final screen so the user can tune the numbers
- Live "if I deposited $X" calculator that splits the deposit across accounts
- Sanity-check warnings (e.g., pricing too low to cover personal expenses)
- localStorage persistence so progress survives a refresh
- Print-friendly final summary

## Tech

- One HTML file. No build step.
- Tailwind CSS via Play CDN
- Alpine.js v3 via CDN
- Inter + DM Serif Display via Google Fonts
- All state in Alpine, persisted to localStorage

## Methodology source

Based on Profit First by Mike Michalowicz. Allocation tables pulled from the official Profit First Instant Assessment PDF and the PFP FAQ document.

## Local development

Just open `index.html` in a browser. Or:

```sh
python3 -m http.server 8000
```

## Deployment

Deployed via GitHub Pages. Any static host will work (Cloudflare Pages, Netlify, S3, etc.) since there is no backend.

## License

Private. Free One Nine Marketing internal tool.
