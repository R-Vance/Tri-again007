# Tri-again007# 457 Retirement Calculator — CalPERS PEPRA

An interactive retirement planning calculator for a California state employee (CalPERS PEPRA) with Roth and Traditional 457 accounts. Built as a single self-contained HTML file — no frameworks, no backend, no login required.

**[Open the Calculator](https://R-Vance.github.io/Tri-again007/)**

---

## What it does

- Projects Roth 457 and Traditional 457b balances from age 33 to retirement at 60.5, assuming an 8% annual return (adjustable)
- Models a contribution ramp from $431/mo to $950/mo, split 50/50 Roth/Traditional
- Calculates CalPERS pension income starting at age 62 (years of service × 2% × final salary)
- Quantifies the 18-month bridge gap between retirement at 60.5 and pension start at 62
- Compares your projected retirement income against an 80% salary replacement target
- Benchmarks your total wealth against US retirement savings percentiles
- Capitalizes your pension at a 4% withdrawal rate to show true total wealth equivalent

## Interactive controls

| Control | What it adjusts |
|---|---|
| Final salary slider | Changes pension calculation and income replacement target |
| Annual return slider | 4%–12%, adjusts all growth projections |
| Service years slider | CalPERS years at age 62 |
| Per-period Roth sliders | Monthly Roth contributions for each 5-year life stage |
| Per-period Traditional sliders | Monthly Traditional contributions for each 5-year life stage |

## Assumptions

- Current age: 33
- Retirement age: 60.5 (December 2053)
- Pension start: 62 (30.5 years of service)
- Starting Roth 457 balance: $7,000
- Starting Traditional 457b balance: $13,000
- CalPERS PEPRA benefit formula: years × 2% × final average pay
- Default return: 8% nominal annual
- No inflation adjustment applied to nominal balances
- Bridge gap calculation assumes 80% salary replacement target for 18 months
- Pension capitalized value uses a 4% safe withdrawal rate
- 30-year withdrawal period used for 457 monthly draw calculation

## How to use locally

Just download `index.html` and open it in any modern browser. No internet connection needed after the first load (Chart.js loads from a CDN on first open).

## How to deploy your own copy

1. Fork or clone this repository
2. Enable GitHub Pages: **Settings → Pages → Deploy from branch → main / root**
3. Your calculator will be live at `https://R-Vance.github.io/retirement-calculator/`

---

*For illustration purposes only. Not financial or investment advice.*
