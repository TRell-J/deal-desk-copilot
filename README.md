# Deal Desk Copilot

A concept prototype for AI-assisted deal desk workflows in regulated, merchant-facing financing environments.

## The problem

Deal desk and merchant-facing sales teams, especially in home improvement financing, make fast, high-stakes framing decisions in live conversations: how to talk about payment options, when to bring up scope expansion, how to handle a price objection, all while staying inside compliance guardrails they may not be able to recite on the spot.

Most tooling built for this moment is either:
- A static script binder nobody opens mid-conversation, or
- A black-box AI assistant that returns an answer without showing its reasoning or leaving anything reviewable behind it.

## The approach

Deal Desk Copilot is a concept prototype that treats explainability, human review, and auditability as first-class product requirements rather than compliance features bolted on after the AI part is done.

Every recommendation shows its reasoning. Every editable output is tracked. Every session produces a reviewable audit trail: what was captured, what the model reasoned, what a human changed, and whether the case needs escalation.

## What this demonstrates

- Product framing for AI-assisted workflows in regulated environments: decision support, not decisioning.
- Designing for auditability from the start: a dedicated audit trail panel rather than a log added afterward.
- Fast, structured prototyping: built end to end as a self-contained interface from intake through recommendation, comparison, and editable scripts.
- Attention to practical product details: WCAG-checked color contrast in both themes, sanitized paste handling on editable fields, and responsive behavior down to mobile.

## What it is

A merchant, such as an HVAC contractor, roofing rep, remodeler, or pools and spas dealer, is mid-conversation with a homeowner and needs help deciding how to talk about financing in real time.

Deal Desk Copilot takes a structured intake, including project category, estimated amount, customer priority, and urgency, and produces:

- A recommended financing conversation approach with plain-English reasoning.
- Scope-expansion or upsell suggestions where relevant.
- An objection-handling script.
- Draft follow-up SMS and email.
- A three-way comparison of financing conversation approaches, not loan products.
- Editable merchant-facing and customer-facing scripts.
- A full audit trail.

It is explicitly scoped as **decision support only**: no credit approvals, no underwriting results, and no lending decisions. That boundary is stated in the UI itself, not just in this README.

## Design principles

This prototype was intentionally shaped around a few principles:

- The AI should help a human operator think, not replace judgment.
- Recommendations should be inspectable, not opaque.
- Auditability should be part of the product interaction, not an afterthought.
- The interface should be useful in a live conversation, not just impressive in a demo.

  ## Spec-to-code approach

This is a prototype-first workflow rather than a traditional long-spec-then-build cycle.

The process moved in tight loops:

1. **Define the workflow, not just the feature.** Before writing anything, the merchant conversation itself was mapped: what information is known at the point of sale, what decision is being made, and what needs to be reviewable afterward.
2. **Draft a lightweight spec.** Inputs, outputs, edge cases, and the compliance boundary (decision support, not decisioning) were defined up front as a short, living spec rather than a lengthy PRD.
3. **Prototype directly against that spec.** The interface was built iteratively in code, with each pass checked against the original intent: does this still support the conversation in real time, and is the reasoning still visible?
4. **Treat the spec and the build as one artifact.** When the interaction model changed, the spec changed with it. Nothing was locked in place before it was tested against the actual experience.
5. **Validate against realistic scenarios**, not just happy-path demos, before considering a feature "done."

The result is a spec that stayed close to the build the entire time, rather than a document written once and handed off.

## What a reviewer should notice

This project is less about a polished production lending workflow and more about the product decisions behind the prototype:

- How the user workflow is scoped.
- How explainability is surfaced in the experience.
- How editable AI outputs are handled.
- How compliance-sensitive thinking shows up in the interface itself.

## Tech stack

Single self-contained HTML file using HTML, CSS, and vanilla JavaScript. No backend, no build step, and no external dependencies.

## Running it

Open `index.html` directly in any browser, or view the live demo via GitHub Pages once enabled for this repo.

## Disclaimer

This is an independent concept prototype using mock data and deterministic sample outputs. It is not affiliated with, built for, or endorsed by any lender, card network, or financial institution. It does not access real credit systems or make lending decisions.


