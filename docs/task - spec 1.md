# Spec-1: Task Statement

AI Assisted Development Process Course

**Title:** Individual Spec Task 1 — Draft Your First Spec Document

**Objective:** Produce a text document that fully specifies the system before any code is written. This is the foundational artifact of Spec-Driven Development (SDD): it forces you to think in contracts and intent before implementation, and it becomes the source of truth an AI coding agent (or teammate) will build against.

**Deliverable:** Two files: one containing the seven sections below in English, each written for the statement presented for the course. Another with the justifications and decisions made.

## Required Sections

- **Contract** — A precise statement of inputs, outputs, and behavior. State exact function/API signatures or interface boundaries, expected data shapes, and error-handling behavior. This section should read like something you could hand to another engineer with zero ambiguity about what "done" means.
- **Why** — One paragraph explaining the problem this solves and who benefits. Ground it in a real need, not a hypothetical.
- **Capabilities** — A bullet list of what the system will actually do, phrased as observable behaviors (not implementation details). Each capability should be testable.
- **Constraints** — Technical, business, or resource limits that shape the solution: performance budgets, language/framework requirements, security rules, timeline, or dependency restrictions.
- **Non-Goals** — Explicit statements of what is intentionally out of scope. This is the section that skips the novice spec-writers, and the one that prevents scope creep and agent hallucination during implementation.
- **Success Signal** — Concrete, measurable criteria for knowing the task is complete: specific tests passing, a metric threshold, a user-observable outcome. Avoid vague statements like "works well."
- **Assumptions** — Anything you're taking for granted (environment, data availability, upstream services, user behavior) that, if false, would break the spec. Flag which assumptions are risky vs. safe.

## Format Requirements

- Maximum 1–2 pages; brevity is graded as a skill, not a shortcut.
- Written in plain language a non-implementer could understand — no code in this first draft.
- Each section header must appear exactly as named above, in order.
- An additional document with justifications: decisions made, tracking of the AI used, self-reviewed aspects, etc.

## Evaluation Criteria

| Criteria | Description | Weight |
|---|---|---|
| Contract clarity | Inputs/outputs/behavior are unambiguous and testable, no implementation leakage | 20% |
| Why justification | Problems and beneficiary are concrete and specific, not generic | 10% |
| Capabilities precision | Each capability is observable and independently verifiable | 15% |
| Constraints completeness | Real technical/business limits are identified, not omitted or invented | 15% |
| Non-goals discipline | Scope boundaries are explicit and prevent obvious over-engineering | 15% |
| Success signal measurability | Criteria are quantifiable or binary (pass/fail), not subjective | 15% |
| Assumptions transparency | Assumptions are named and risk-ranked, not buried or missing | 10% |

A passing spec should be detailed enough that a second person — or an AI agent — could implement the feature from the document alone without needing to ask clarifying questions about scope, done-ness, or edge-case behavior. That is the practical bar for this assignment.

This is a level 3 AI assignment. Use of AI to iterate specification, keeping track of modifications and justifications, self-review of ambiguities, omissions, contradictions, and anti-patterns.