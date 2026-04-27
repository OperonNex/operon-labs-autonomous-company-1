# Operon Labs: Autonomous Company #1

*A company where no human writes the code.*

---

## Overview

This repository hosts an **autonomous company** experiment: AI agents own development, execution, and iteration. The human operator sets direction and constraints, not implementation details.

**v2 product direction:** help **indie hackers** go from “I have an MVP” to “it runs on a **VPS**” with a clear, repeatable way to **wire up** the server: deploy, domains/TLS, process supervision, and basic ops—without becoming a second full-time job.

The outcome should feel like: *connect your repo and credentials, get a small production-shaped setup you can grow or throw away.*

---

## Audience

- Operators and researchers who want to explore **agent-only** software development lifecycles.
- Teams evaluating how much human steering is still required when agents own implementation, QA, and iteration.
- **Indie hackers** and solo builders who want a credible path from MVP to a small production setup on a VPS, without a second full-time ops role.
- Anyone following this experiment to learn failure modes, limits, and what “autonomous” can mean in practice.

---

## Value proposition

- A **documented, transparent** test bed for running a product with agents—not a pitch deck, but a working record of constraints, decisions, and outcomes.
- A place to see whether a codebase can be **sustained over time** without hand-written operator code, and what breaks first when it can’t.
- For the v2 focus: **less time from “it works on my machine” to “it runs on a VPS”** with opinionated, automatable wiring—honest about single-server MVP scope, not a cloud platform in disguise.
- Honest scope: you get **clarity on autonomy boundaries**, not a guarantee of a finished product.

---

## Why this focus

Solo builders often ship a prototype fast, then stall on the “boring but sharp” work: reverse proxy, HTTPS, restarts, logs, backups, and a deployment story that is not “SSH and hope.” This project exists to productize that path for MVPs: **opinionated, automatable, small.**

The autonomous company angle stays: the **system** (agents + tooling) builds and maintains what ships; the operator does not hand-author product code.

---

## How work happens

| Role | Responsibility |
|------|----------------|
| **Operator** | Product direction, constraints, review—not day-to-day implementation |
| **Agents** | Tasks, code, structure, iteration, and validation where applicable |

Conventions: no manual coding from the operator; high-level direction only; agent-driven execution.

---

## v2 goals (MVP / VPS)

- **Reduce time-to-production** for a small app on a single VPS
- **Document and automate** the standard glue: app runtime, reverse proxy, TLS, env/config, health checks, deploy hooks
- **Stay honest about scope:** one VPS, MVP-grade—not a full cloud platform

Non-goals for v2 (unless direction changes): multi-region, enterprise compliance programs, or hardware businesses.

---

## Stricter internal specifications checklist

Use this as a non-negotiable bar for work inside this experiment:

- [ ] No manual implementation of product code; change flows through the agent system.
- [ ] Direction and constraints are explicit before agents execute; no implicit “just fix it” work.
- [ ] All meaningful decisions (scope, structure, major trade-offs) are **recorded** in-repo where applicable.
- [ ] Outcomes are reviewable: what shipped, what failed, and what was learned.
- [ ] If something is production-sensitive, it is **called out** and not treated as ready without separate validation.

When you are ready to **lock product choices** (complements the list above; fill in under `/docs` as the build solidifies):

- **Target stack and OS** (e.g. Linux only; which distros or a single golden image)
- **Secrets and credentials model** (how repo, CI, and VPS credentials are expected to flow; short threat model)
- **Supported app shapes** (e.g. one container vs bare process; static sites; databases on-box vs managed)
- **SLOs for “MVP”** (backup frequency, restore drill, log retention, acceptable downtime for v1)
- **Agent boundaries** (what agents may change without review vs what requires human sign-off)

None of the product-hardening bullets need to be fully specified until there is a concrete build; they are a checklist for when the product tightens.

---

## Repository structure

This will evolve. Expected areas:

- `/project` — the product (CLI, config, or services that implement the VPS wiring)
- `/agents` — agent definitions and responsibilities
- `/logs` — decisions, outcomes, and failures
- `/docs` — deeper notes, runbooks, and (when added) the stricter internal specifications above

---

## Status

**Phase:** v2 direction locked at README level; implementation and internal specs to follow.

---

## Transparency

This is an experiment. Expect rough edges, incomplete automation, and direction changes. That is part of the process.

---

## License

TBD
