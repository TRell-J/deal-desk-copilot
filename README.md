# Deal Desk Copilot

A concept prototype exploring decision-support tooling for point-of-sale merchant financing conversations — built as a product and UX case study, not a production system.

## What it is

A merchant (HVAC contractor, roofing rep, remodeler, pools & spas dealer) is mid-conversation with a homeowner and needs help deciding how to talk about financing in real time. Deal Desk Copilot takes a structured intake — project category, estimated amount, customer priority, urgency — and produces:

- A recommended financing conversation approach with plain-English reasoning
- Scope-expansion / upsell suggestions where relevant
- An objection-handling script
- Draft follow-up SMS and email
- A three-way comparison of financing conversation approaches (not loan products)
- Editable merchant-facing and customer-facing scripts
- A full audit trail — captured inputs, AI reasoning summary, human edits, approval state, and escalation flags

It's explicitly scoped as decision support only: no credit approvals, no underwriting results, no lending decisions. That boundary is stated in the UI itself, not just in this README.

## Why this exists

Built to explore what "AI-native" product thinking looks like when explainability, audit trails, and human-in-the-loop review are treated as first-class product requirements from the start — not compliance features bolted on after the fact.

## Features

- KPI header: estimated time saved, potential ticket uplift, merchant confidence, human-review-required status
- Structured merchant intake form with quick-load example scenarios (HVAC emergency replacement, roofing insurance gap, kitchen remodel upsell)
- Deterministic recommendation engine — scenario-aware, with a procedural (non-decorative) loading state
- Financing conversation comparison table with customer-fit and review-flag columns
- Inline-editable merchant/customer scripts, with paste forced to plain text (no injected markup or styling)
- Full audit trail panel with an exportable JSON log
- Light/dark theme with a visible toggle, responsive down to mobile, WCAG-checked color contrast on both themes

## Tech stack

Single self-contained HTML file — HTML, CSS, and vanilla JavaScript. No backend, no build step, no dependencies.

## Running it

Open `deal-desk-copilot.html` directly in any browser — or view it live via GitHub Pages once enabled for this repo.

## Disclaimer

This is an independent concept prototype using mock data and deterministic sample outputs. It is not affiliated with, built for, or endorsed by any lender, card network, or financial institution, and does not access real credit systems or make lending decisions.
