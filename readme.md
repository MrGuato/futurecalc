# FutureCalc — Smart & Secure Calculator

*A modern, open-source calculator for building wealth safely - security‑first, transparent, and client‑only.*

[![Made With Love](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F-by%20Jonathan-red)](https://github.com/MrGuato)
[![Page Deployment](https://github.com/MrGuato/futurecalc/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/MrGuato/futurecalc/actions/workflows/pages/pages-build-deployment)
[![Lint Status](https://github.com/MrGuato/futurecalc/actions/workflows/lint.yml/badge.svg)](https://github.com/MrGuato/futurecalc/actions/workflows/lint.yml)
[![CodeQL Analysis](https://github.com/MrGuato/futurecalc/actions/workflows/codeql.yml/badge.svg)](https://github.com/MrGuato/futurecalc/actions/workflows/codeql.yml)
[![Known Vulnerabilities](https://snyk.io/test/github/MrGuato/futurecalc/badge.svg)](https://snyk.io/test/github/MrGuato/futurecalc)
[![Dependabot](https://img.shields.io/badge/Dependabot-enabled-brightgreen?logo=dependabot)]()
[![Scorecard supply-chain security](https://github.com/MrGuato/futurecalc/actions/workflows/scorecard.yml/badge.svg)](https://github.com/MrGuato/futurecalc/actions/workflows/scorecard.yml)
![GitHub Repo stars](https://img.shields.io/github/stars/MrGuato/futurecalc?style=social)
[![Last Commit](https://img.shields.io/github/last-commit/MrGuato/futurecalc)]()

**Live Demo:** [FutureCalc.io](<https://mrguato.github.io/futurecalc/>)
**Report Card:** [Open SSF Report Card](<https://scorecard.dev/viewer/?uri=github.com/MrGuato/futurecalc&sort_by=check-score&sort_direction=desc>)

---

## What is FutureCalc?
FutureCalc is a lightweight, privacy‑respecting tool that helps you:
- Split each paycheck between savings and investing
- Build a 6‑month emergency fund
- Understand compounding with clear visuals
- Explore debt payoff, mortgages, and DCA for crypto

Everything runs locally in your browser. No tracking. No backend. Open source.

---

## Features

Core
- Paycheck planner with percentage sliders and direct input
- Emergency fund target and progress bar (6× monthly expenses by default)
- Growth projection with Investing vs Savings chart
- Contributions vs growth breakdown and time‑based milestones
- Dark mode, responsive UI, accessible colors and keyboard navigation

Calculators
- Debt payoff
  - Avalanche and Snowball strategies
  - Amortization with extra payments
  - Time to payoff, interest saved
  - Balance‑over‑time chart and CSV export
- Mortgage
  - Payment calculation and full amortization
  - Extra payments and time‑to‑payoff
  - 80% LTV milestone estimate (PMI proxy)
  - Balance‑over‑time chart and CSV export
- Crypto (DCA)
  - Periodic buys with fee input
  - Average cost, ending value, max drawdown
  - Portfolio value vs contributions chart and CSV export

Privacy & Performance
- 100% client‑side, no data collection
- LocalStorage for convenience
- No frameworks required, fast load over a CDN

---

## Why FutureCalc?
Most online calculators are either black boxes or trade convenience for privacy. FutureCalc is:
- Open‑source and auditable
- Explicit about formulas and assumptions
- Built with secure engineering practices from the start

> Educational tool only — not financial advice. Returns are hypothetical.

---

## Security Engineering Focus
Showcasing secure‑by‑default front‑end practices:

- Client‑only architecture
  - No cookies, no sessions, no tracking
  - Inputs persist only in LocalStorage
- Secure coding standards
  - No unsafe `eval`
  - Scoped functions and listeners
  - Defensive parsing and bounds checking on user inputs
- Supply chain hygiene
  - Dependabot for updates
  - CodeQL for static analysis
  - Linting and formatting in CI
  - OpenSSF Report Card
- Repo hygiene
  - MIT License
  - SECURITY.md for vulnerability reporting
  - Minimal, auditable third‑party usage (Chart.js via CDN)

---

## Architecture
- Single‑page app: `index.html` with vanilla HTML/CSS/JS
- ES‑module style organization within one script
- Charts via Chart.js
- No build step; GitHub Pages ready

---

## Getting Started

Local
- Clone the repo
- Open `index.html` in a modern browser

GitHub Pages (https://mrguato.github.io/futurecalc/)
- Open Browser for Browser Based Calculator

---

## Methods and Assumptions (Finance)
- Compound growth: future value with periodic contributions
- Savings APY and investment return applied per‑period
- Debt payoff:
  - Monthly interest accrual, minimums first
  - Extra payment allocated per chosen strategy
- Mortgage:
  - Standard amortization `M = P·i·(1+i)^n / ((1+i)^n − 1)`
  - Extra payments reduce principal, shortening term
  - 80% LTV milestone as a PMI proxy (informational only)
- Crypto DCA:
  - Units from contribution net of fee
  - Average cost, ending value, max drawdown
  - Optional simulated path for illustration

---

## Roadmap
- [x] Add UI Changes for Dark & Light Modes
- [x] Add Debt Calculator
- [x] Add Crypto Calculator
- [x] Add Mortgage Calculator
- [x] Add Graphs
- [ ] Scenario comparison (e.g., 10% vs 15% investing)
- [ ] Real vs nominal returns (inflation toggle)
- [ ] FAQ and “Methods” page with citations
- [ ] Printable reports for projections and schedules

---

## Security Policy
See SECURITY.md for how to report a vulnerability.

---

## License
MIT License © 2025 Jonathan DeLeon

---

## Contributing
Contributions are welcome. Please open an issue or submit a pull request with clear scope and validation steps.
