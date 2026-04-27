# Operon Labs: Autonomous Company #1

*A company where no human writes the code.*

---

## Overview

This repository hosts an **autonomous company** experiment: AI agents own development, execution, and iteration. The human operator sets direction and constraints, not implementation details.

**v2 product direction:** help **indie hackers** go from “I have an MVP” to “it runs on a **VPS**” with a clear, repeatable way to **wire up** the server: deploy, domains/TLS, process supervision, and basic ops—without becoming a second full-time job.

The outcome should feel like: *connect your repo and credentials, get a small production-shaped setup you can grow or throw away.*

---

## Why this focus

Solo builders often ship a prototype fast, then stall on the “boring but sharp” work: reverse proxy, HTTPS, restarts, logs, backups, and a deployment story that is not “SSH and hope.” This project exists to productize that path for MVPs: **opinionated, automatable, small.**

The autonomous company angle stays: the **system** (agents + tooling) builds and maintains what ships; the operator does not hand-author product code.

---

## How work happens

| Role | Responsibility |
|------|------------------|
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

## Stricter internal specifications (still to document)

The public README is the product **direction**. Tighter, internal-style specs should be added when you are ready to lock choices—suggested areas:

- **Target stack and OS** (e.g. Linux only; which distros or a single golden image)
- **Secrets and credentials model** (how repo, CI, and VPS credentials are expected to flow; threat model in one page)
- **Supported app shapes** (e.g. one container vs bare process; static sites; databases on-box vs managed)
- **SLOs for “MVP”** (backup frequency, restore drill, log retention, acceptable downtime for v1)
- **Agent boundaries** (what agents may change without review vs what requires human sign-off)

None of the above need to be invented here until there is a concrete build; this list is a checklist for when the product hardens.

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
