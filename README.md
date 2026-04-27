# Operon Labs: Autonomous Company #1
*A company where no human writes the code.*

---

## Overview

This repository documents an ongoing experiment.

The goal is to run a software project where AI agents handle development, execution, and iteration.

I do not write code.

I only provide direction.

Everything else is done by the system.

---

## Audience

- Operators and researchers who want to explore **agent-only** software development lifecycles.
- Teams evaluating how much human steering is still required when agents own implementation, QA, and iteration.
- Anyone following this experiment to learn failure modes, limits, and what “autonomous” can mean in practice.

---

## Value proposition

- A **documented, transparent** test bed for running a product with agents—not a pitch deck, but a working record of constraints, decisions, and outcomes.
- A place to see whether a codebase can be **sustained over time** without hand-written code, and what breaks first when it can’t.
- Honest scope: you get **clarity on autonomy boundaries**, not a guarantee of a finished product.

---

## Stricter internal specifications checklist

Use this as a non-negotiable bar for work inside this experiment:

- [ ] No manual implementation of product code; change flows through the agent system.
- [ ] Direction and constraints are explicit before agents execute; no implicit “just fix it” work.
- [ ] All meaningful decisions (scope, structure, major trade-offs) are **recorded** in-repo where applicable.
- [ ] Outcomes are reviewable: what shipped, what failed, and what was learned.
- [ ] If something is production-sensitive, it is **called out** and not treated as ready without separate validation.

---

## Concept

Traditional software development requires teams of engineers, product managers, and operators.

This experiment explores a different approach:

> Can a company operate with autonomous agents handling the entire lifecycle?

From planning to implementation to iteration.

---

## Rules

The experiment follows strict constraints:

- No manual coding
- No direct intervention in implementation
- Only high-level decisions and constraints
- All execution is agent-driven

---

## What the Agents Handle

- Task creation and prioritization
- Code generation and modification
- Project structure decisions
- Iteration and improvements
- Basic QA and validation (where applicable)

---

## Role of the Operator

- Define direction
- Set constraints
- Review outcomes
- Adjust strategy when necessary

No direct implementation.

---

## Current Status

**Phase:** Initialization

The system is being set up and initial workflows are being defined.

---

## Goals

- Validate whether agents can maintain a codebase over time
- Observe failure points and limitations
- Identify what level of autonomy is realistically achievable
- Understand how much human input is actually required

---

## Transparency

This is not a polished product.

Expect:
- mistakes
- broken implementations
- unexpected behavior
- incomplete features

That is the point of the experiment.

---

## Structure

This repository will evolve over time.

Expected components:

- `/project` → the product being built
- `/agents` → agent definitions and responsibilities
- `/logs` → notable decisions, outcomes, and failures
- `/docs` → experiment notes and observations

---

## Updates

Progress, failures, and insights will be documented continuously.

This is a live experiment.

---

## Disclaimer

This project is experimental.

Nothing here should be considered production-ready.

---

## License

TBD
