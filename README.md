# CSRD Readiness Assessment Framework

A browser-based, zero-dependency interactive tool that helps companies evaluate
their preparedness for the **Corporate Sustainability Reporting Directive (CSRD)**
across all 10 European Sustainability Reporting Standards (ESRS) disclosure areas.

Built as a portfolio project targeting green-tech, ESG SaaS, and PropTech companies
operating in the EU sustainability reporting space.

---

## 🌿 Live Demo

> Open `https://jacob-hub-esg.github.io/csrd-framework/` directly in any modern browser — no install, no server required.

---

## 📋 Overview

The CSRD mandates that thousands of EU companies publicly disclose sustainability
performance across Environmental, Social, and Governance (ESG) dimensions using ESRS
standards. This tool operationalises that framework into an interactive, self-guided
assessment that:

- Walks users through **10 ESRS sections** (~40 weighted questions)
- Generates a **real-time readiness score** (0–100) per section and overall
- Surfaces **priority gaps** and **tailored action recommendations**
- Displays a **CSRD compliance timeline** for different company categories

---

## ✨ Features

### Multi-Step Assessment Flow
- Company onboarding (name, sector, size, country)
- Section-by-section questionnaire with animated progress tracking
- Skip and back navigation for non-linear completion

### Scoring Engine
- Each question carries a **weighted score** (10–35 pts) reflecting regulatory significance
- Per-section scores computed as `(earned weight / total weight) × 100`
- Overall score aggregated across all 10 ESRS sections
- Readiness tiers: **CSRD Ready** (≥80) · **On Track** (≥60) · **Developing** (≥40) · **Action Required** (<40)

### Results Dashboard
- **Pillar scores** for Environment (E1–E5), Social (S1–S4), and Governance (G1)
- **Section-by-section breakdown** with visual progress bars
- **Top 3 priority gaps** with specific unanswered disclosures highlighted
- **Action recommendations** calibrated per section (Foundation / Intermediate / Advanced)
- **CSRD compliance timeline** showing the 2024–2028 phased rollout

### Design
- Dark-mode UI with `DM Mono` + `Syne` typography
- Smooth fade-in transitions between steps
- Fully responsive — single-column layout on mobile
- Zero external JavaScript dependencies (vanilla JS + CSS only)

---

## 🗂️ ESRS Coverage

| Code | Area        | Topic                            |
|------|-------------|----------------------------------|
| E1   | Environment | Climate Change                   |
| E2   | Environment | Pollution                        |
| E3   | Environment | Water & Marine Resources         |
| E4   | Environment | Biodiversity & Ecosystems        |
| E5   | Environment | Resource Use & Circular Economy  |
| S1   | Social      | Own Workforce                    |
| S2   | Social      | Workers in Value Chain           |
| S3   | Social      | Affected Communities             |
| S4   | Social      | Consumers & End-Users            |
| G1   | Governance  | Business Conduct & Governance    |

---

## 🛠️ Tech Stack

| Layer     | Technology                                      |
|-----------|-------------------------------------------------|
| Runtime   | Vanilla JavaScript (ES6+)                       |
| Styling   | Plain CSS — Grid, custom properties, animations |
| Fonts     | Google Fonts (DM Mono, Syne)                    |
| Rendering | DOM manipulation — no framework                 |
| Build     | None — single `.html` file, runs anywhere       |

---

## 🚀 Getting Started

```bash
# No installation needed — just clone and open
git clone https://github.com/jacob-hub-esg/csrd-framework
cd csrd-framework
open https://jacob-hub-esg.github.io/csrd-framework/
```

Or serve it statically:

```bash
npx serve .
# → http://localhost:3000
```

---

## 🧠 Methodology & Data Sources

- **ESRS framework**: EFRAG ESRS Set 1 (delegated act, July 2023)
- **Question weights**: Calibrated against CSRD disclosure materiality guidance
- **Action recommendations**: Aligned with GRI Standards, TCFD, UN Guiding Principles,
  ISO 14001/45001, and SBTi
- **Compliance timeline**: European Commission phased rollout (Directive 2022/2464/EU)

---

## 🔮 Roadmap

- [ ] PDF / CSV export of assessment results
- [ ] Sector-specific question weighting (Real Estate vs Manufacturing etc.)
- [ ] Double materiality assessment module
- [ ] Multi-user collaboration with shared state
- [ ] EU Taxonomy alignment scoring integration
- [ ] Embeddable API for third-party ESG platforms

---

## 🌍 Context & Motivation

This project is part of a green-tech portfolio series exploring tooling at the
intersection of sustainability regulation and developer experience. The CSRD represents
one of the most significant expansions of corporate ESG disclosure requirements globally,
and accessible tooling for SMEs is still nascent.

Related tools in this series:
- `building-emissions-tool` — GHG Protocol building carbon calculator with EU
  benchmarking and net-zero pathway modelling
- `CO2BenchmarkCalculator` — Commercial real estate carbon intensity estimator
  with BREEAM / EU Taxonomy comparisons

---

## 📄 License

MIT — free to use, adapt, and build upon.

---

*Built with 🌿 for the EU green transition.*
