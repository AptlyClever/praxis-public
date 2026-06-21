# Praxis Public

Praxis Public is a curated, public-readable slice of the Praxis workflow model.

It exists so humans and agents can understand the Control Alt workflow vocabulary, evidence chain, and public-safe operating model without access to private implementation repos, private operational records, runtime logs, LAN details, credentials, or unpublished product work.

## What this repo is

Praxis Public is:

- a public orientation surface,
- a readable object-model reference,
- a source of public-safe examples,
- a corpus for testing agent comprehension,
- a bridge between human planning and agent execution.

## What this repo is not

Praxis Public is not:

- the private operational Praxis ledger,
- a deployment authority system,
- a substitute for private implementation context,
- a place for secrets, logs, runtime proofs, internal paths, LAN details, or unfinished private work,
- an instruction to merge, deploy, restart, publish, or operate services.

## Praxis lifecycle

```text
Intent → Directive → Praxis Record → Implementation PR / Evaluation Run → Report / Readout → Review → Outcome
```

Relay may transport or archive workflow artifacts. Praxis owns the object model and evidence chain.

## First-class Praxis object kinds

| Kind | Meaning |
| --- | --- |
| Campaign | Broad coordinated effort spanning lanes, agents, repos, standards, and checkpoints |
| Beacon | Current navigation, state, and evidence map for a Campaign or Strand |
| Strand | Bounded line of work inside a Campaign |
| Fiber | Small identifiable work unit that advances a parent Strand |
| Directive | Instruction object telling an agent or implementer what to do, under what boundaries, with what validation and reporting expectations |
| Readout | Recorded result from a bounded evaluation run |
| Probe | Reusable observation-first check |
| Protocol | Repeatable procedure composed of runnable steps |
| Doctrine | Durable reusable guidance |
| Imprint | Durable rationale or decision trace |

## Supporting workflow artifacts

| Artifact / concept | Meaning |
| --- | --- |
| Praxis Record | Preserved execution/evidence ledger entry |
| Report | Completion/evidence summary |
| Implementation PR | Code-change vehicle in an implementation repository |
| Relay | Transport/archive layer for workflow artifacts; not workflow authority |

## Recommended load order

For humans or agents entering a workstream midstream:

1. Beacon — where are we?
2. Campaign — what is the larger effort?
3. Strand — which line of work are we in?
4. Fiber — what concrete piece are we doing?
5. Directive — what exactly was the agent told to do?
6. Praxis Record / Report / Readout — what happened, what proved it, and what did we learn?

Beacon is the front door. Directive is the work order. Praxis Record, Report, and Readout are the evidence trail.

## Seed contents

This initial public seed includes:

- `PUBLIC_PRIVATE_BOUNDARY.md` — what belongs in public Praxis vs private Praxis.
- `objects/imprints/praxis-object-type-translation-map.md` — human-readable translation map for Praxis object types.
- `objects/strands/praxis-public-solution.md` — public-safe Strand summary for building this public layer.
- `objects/campaigns/control-alt-development-workflow-flexibility.md` — public-safe Campaign summary for agent/workflow flexibility.
- `objects/doctrines/praxis-evidence-chain.md` — public-safe evidence-chain doctrine.
- `objects/probes/public-praxis-readiness.md` — observation-only readiness probe for this public surface.
- `prompts/agent-readonly-comprehension.md` — first read-only agent comprehension prompt.

## Authority boundary

Nothing in this public repo grants authority to access private repos, modify implementation code, merge PRs, deploy software, restart services, operate devices, change network or Docker state, publish private material, or perform destructive actions.

Public Praxis is orientation and reusable public canon. Private Praxis remains the operational ledger.
