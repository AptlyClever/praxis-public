# Current Operating Model

Orientation for agents entering the Control Alt workflow. This document is public-safe context only.
Private Praxis retains operational authority.

## Authority map

| Component | Role |
| --- | --- |
| **Private Praxis** | Workflow authority and evidence ledger. All Directives originate here. |
| **Praxis Public** | Public-safe orientation only. No implementation authority. |
| **Axiom Work Compass** | Intended owner-facing reducer and operating surface. Not current implementation authority. |
| **ctrl-alt-standards** | Context and reference. Active for a task only when private Praxis imports or points to it. |
| **Handoff / Relay** | Compatibility layer only. Not the future workflow center. |

## Rules agents must hold

- **Implementation requires a private Praxis Directive or task packet.** Public orientation is not a work order.
- **Axiom Work Compass is the intended owner-facing surface** for Praxis-backed work. It is not yet implementation authority; treat it as a design direction, not a current source of authority.
- **ctrl-alt-standards is reference only** unless private Praxis explicitly imports or points to it for the current task.
- **Handoff / Relay is compatibility only.** Do not treat it as the workflow center or the intended future path.
- **Artifact handling requires Praxis policy** before implementation. Do not assume artifact destinations, formats, or storage locations.
- **Direct API runner / patch-runner work is downstream of Praxis authority.** It executes under Praxis Directives and must not become a second workflow brain or independent authority source.

## What this means for a fresh agent

1. Load Praxis Public for orientation, vocabulary, and object model.
2. Do not act on Praxis Public alone — it is context, not authorization.
3. Request or receive a private Directive from private Praxis before proposing or executing any implementation.
4. Treat Axiom, ctrl-alt-standards, Handoff/Relay, and runner work as downstream components. None of them grant authority.
