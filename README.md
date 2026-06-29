# Blocksure Website

Marketing website for **Blocksure** — the skills-economy infrastructure: quality-assured,
machine-readable Rich Skill Descriptors (RSDs), blockchain-secured credentials, and a live
microcredentials marketplace.

Built as a static, dependency-free multi-page site (plain HTML + CSS) from the Claude Design
redesign handoff. No build step required — open `index.html` or serve the folder with any static
host.

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Home — hero, metrics, problem, infrastructure stack, ecosystem, offerings, CTA |
| `platform.html` | Platform overview — all 14 products |
| `marketplace.html` | Microcredentials Marketplace (flagship) |
| `solutions.html` | Solutions for RTOs, Employers, Government, Individuals |
| `simulab.html` | Simulab — AI Simulation Builder |
| `skills-database.html` | Skills Database & OSMT |
| `credentials.html` | Digital Credentials & Badges |
| `skills-bridge.html` | Skills Bridge — skills-based hiring |
| `micropromote.html` | Micropromote — Social Media Studio |
| `strategy.html` | Strategy Development System |

Shared site navigation and footer are inlined into every page (the nav highlights the active
section). Brand assets live in `assets/`.

## Design system

- **Type:** Bricolage Grotesque (display), Hanken Grotesk (body), JetBrains Mono (labels) — loaded from Google Fonts
- **Core colors:** ink `#0F1535`, navy `#0B1430`, blue `#5B8DEF`, violet `#8B5CF6`, teal `#1FA6BC`
- **Layout:** 1240px max content width, responsive grids, `clamp()` fluid spacing/type

## Running locally

```bash
# any static server, e.g.
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deployment

Any static host (GitHub Pages, Netlify, Cloudflare Pages, S3, etc.). Publish the repository root;
`index.html` is the entry point.
