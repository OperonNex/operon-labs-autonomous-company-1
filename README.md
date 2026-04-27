# Operon Labs: Autonomous Company #1
*A company where no human writes the code.*

This repository is the home base for a **builder-focused, agent-run software business**: direction comes from a human operator; implementation and iteration are done by the system.

---

## Audience

We design for **indie hackers**—solo founders and very small teams who:

- ship their own products without a traditional eng org
- want leverage from agents without losing control of scope and quality
- care about clear constraints, fast iteration, and honest tradeoffs
- are comfortable with an experimental, evolving codebase

If that sounds like you, the docs here are meant to be readable, opinionated, and useful as a runbook—not just marketing copy.

---

## Value proposition

- **You set direction, not diffs.** You define what we’re building and what “good” means; agents own implementation, refactors, and day-to-day changes.
- **A real product loop.** The goal is a **for-profit, digital-only** business: shipping meaningful functionality, not a one-off demo.
- **Guardrails by default.** Work stays within legal and ethical bounds (no gambling products, no deceptive or exploitative systems, no illegal or widely restricted handling).
- **Transparent ops.** Progress, mistakes, and decisions are visible so you can steer without micromanaging the codebase.

---

## Stricter internal specifications (checklist)

Use this list for **every non-trivial change** so agent output stays reviewable and mergeable.

- [ ] **Scope** — One clear intent (user story or single sentence); out-of-scope items called out.
- [ ] **Acceptance criteria** — Observable outcomes, testable in principle (manual or automated).
- [ ] **Public contracts** — APIs, env vars, and CLI flags documented where they’re introduced or changed.
- [ ] **Safety and compliance** — No new data handling or flows that violate the constraints above; note “none” if N/A.
- [ ] **Tests** — New behavior covered where the repo already has tests; new critical paths get at least a minimal check.
- [ ] **Rollback / feature flags** — If a change is risky, document how to disable or revert it.
- [ ] **Observability** — Log or metric hooks for new failure paths when the app already has patterns for them.

Tightening these over time is expected. When in doubt, add a line to `/logs` or `/docs` so the next run has context.

---

## Overview

The goal is to run a software project where **AI agents** handle development, execution, and iteration. The operator does not write code—only **direction, constraints, and review**.

---

## What the agents handle

- Task creation and prioritization
- Code generation and modification
- Project structure decisions
- Iteration and improvements
- Basic QA and validation (where applicable)

---

## Role of the operator

- Define direction
- Set constraints
- Review outcomes
- Adjust strategy when necessary

No direct implementation.

---

## Current status

**Phase:** Initialization

The system is being set up and initial workflows are being defined.

---

## Repository structure (expected)

This tree will grow over time. Planned layout:

- `/project` → the product being built
- `/agents` → agent definitions and responsibilities
- `/logs` → notable decisions, outcomes, and failures
- `/docs` → experiment notes and observations

---

## Transparency

This is not a polished product. Expect mistakes, broken implementations, unexpected behavior, and incomplete features. That is the point of the experiment.

---

## License

TBD
