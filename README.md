# Deal Desk Copilot

**A case study in AI solutioning for deal desk professionals.**

## The problem

Deal desk and merchant-facing sales teams — especially in home improvement financing — make fast, high-stakes framing decisions in live conversations: how to talk about payment options, when to bring up scope expansion, how to handle a price objection, all while staying inside compliance guardrails they can't always recite on the spot. Most tooling built for this moment is either a static script binder nobody opens mid-conversation, or a black-box "AI assistant" that hands back an answer without showing its reasoning or leaving anything reviewable behind it.

## The approach

Deal Desk Copilot is a concept prototype that treats explainability, human review, and auditability as first-class product requirements — not compliance features bolted on after the AI part is "done." Every recommendation shows its reasoning, every editable output is tracked, and every session produces a reviewable audit trail: what was captured, what the model reasoned, what a human changed, and whether the case needs escalation.

## What this demonstrates

- **Product framing for AI-assisted workflows in regulated environments** — decision support, not decisioning; the tool never claims to approve, underwrite, or predict credit outcomes.
- **Designing for auditability from the start** — a dedicated audit trail panel (timestamped inputs, reasoning summary, human edits, approval state, escalation flags), not a log tacked on afterward.
- **Fast, structured prototyping** — built end-to-end as a single self-contained interface, from intake form through recommendation, comparison, and editable scripts.
- **Attention to real production details** — WCAG-checked color contrast in both themes, sanitized paste handling on editable fields, responsive layout down to mobile.

## What it is

A merchant (HVAC contractor, roofing rep, remodeler, pools & spas dealer) is mid-conversation with a homeowner and needs help deciding how to talk about financing in real time. Deal Desk Copilot takes a structured intake — project category, estimated amount, customer priority, urgency — and produces:

- A recommended financing conversation approach with plain-English reasoning
- Scope-expansion / upsell suggestions where relevant
- An objection-handling script
- Draft follow-up SMS and email
- A three-way comparison of financing conversation approaches (not loan products)
- Editable merchant-facing and customer-facing scripts
- A full audit trail

It's explicitly scoped as decision support only: no credit approvals, no underwriting results, no lending decisions. That boundary is stated in the UI itself, not just here.

## Tech stack

Single self-contained HTML file — HTML, CSS, and vanilla JavaScript. No backend, no build step, no dependencies.

## Running it

Open `deal-desk-copilot.html` directly in any browser, or view the live demo via GitHub Pages once enabled for this repo.

## Disclaimer

This is an independent concept prototype using mock data and deterministic sample outputs. It is not affiliated with, built for, or endorsed by any lender, card network, or financial institution, and does not access real credit systems or make lending decisions.
