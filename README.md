# Responin Landing Page V3

Static bilingual website for **Responin** — an AI operations agent for busy business teams.

V3 combines:

- **Landing page V2** as the concise, high-conversion homepage.
- **Landing page V1** as the deeper product, pricing, legal, and bilingual infrastructure.
- System-design positioning from `psatriyo/responin-system-design`: LLMs reason/draft; systems authorize, meter, execute, and log.

## Pages

| Page | Purpose |
|---|---|
| `index.html` | Short V2-style homepage: problem, 15-second demo, workflows, operating loop, safety, CTA |
| `learnmore.html` | Detailed product information, use cases, industries, comparison, FAQ |
| `pricing.html` | Modular Indonesian-market pricing and calculator |
| `privacy.html` | Bilingual privacy policy |
| `termsofuse.html` | Bilingual terms of use |

## Stack

Plain static site:

- HTML
- CSS
- vanilla JavaScript
- no build step
- bilingual EN/ID via `i18n.js` and `i18n-legal.js`

## QA

Run from the repo root:

```bash
node --check app.js
node --check i18n.js
node validate-i18n.js
node validate-site.js
node tests/validate-landing-architecture.js
node tests/validate-pricing-calculator.js
```

## Local preview

```bash
python3 -m http.server 8080
```

Then open <http://localhost:8080>.
