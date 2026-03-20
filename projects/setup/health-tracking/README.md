---
project: setup-health-tracking
status: pending
created: auto
tags: [setup]
---

# Setup: Health Tracking

## Goal

Set up persistent health context so your AI can track biomarkers, supplements, and health decisions over time.

## Steps

- [ ] **Create health directory** — `knowledge/health/`
- [ ] **Biomarkers** — Record your latest blood work in `knowledge/health/biomarkers/{year}.md`
- [ ] **Supplements** — Document your current stack in `knowledge/health/supplements/current.md`
- [ ] **Genetic profile** — If available, record key markers (APOE, Lp(a), etc.)
- [ ] **Targets** — Define your biomarker targets and thresholds
- [ ] **Optional: Staleness alerts** — Configure an automation to alert when data is stale

## Why Track Health in Your AI Context?

- Your AI can flag supplement interactions before you add something new
- Lab results get compared against your personal history, not just population averages
- Health decisions are logged with reasoning (journal entries)
- Genetic context informs all recommendations
