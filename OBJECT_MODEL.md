# Praxis Object Model

First-class object kinds in the Praxis workflow ledger.

## Lifecycle

```
Signal → Response → Campaign → Aim → Strand → Stint → Grant → Execution → Resolution
```

## Object kinds

| Kind | Type value | Meaning |
| --- | --- | --- |
| **Signal** | `praxis.signal` | Low-authority captured idea or observation preserved for later triage |
| **Campaign** | `praxis.campaign` | Coordinated multi-lane effort spanning agents, repos, and decision checkpoints |
| **Beacon** | `praxis.beacon` | Current navigation, state, and evidence map for a Campaign or Strand |
| **Strand** | `praxis.strand` | A continuing line of attention kept open toward an outcome |
| **Fiber** | `praxis.fiber` | Small identifiable work unit that advances a parent Strand |
| **Directive** | `praxis.directive` | Instruction object: authorized action, boundaries, validation, stop conditions |
| **Readout** | `praxis.readout` | Recorded result from a bounded evaluation run |
| **Probe** | `praxis.probe` | Reusable check — observation-first pass/fail evidence |
| **Protocol** | `praxis.protocol` | Repeatable procedure composed of steps |
| **Doctrine** | `praxis.doctrine` | Reusable guidance that outlives a single task |
| **Imprint** | `praxis.imprint` | Durable rationale or decision trace |

## Object metadata schema

| Field | Example | Notes |
| --- | --- | --- |
| `id` | `strand-praxis-public-solution` | Human-readable slug |
| `type` | `praxis.strand` | `praxis.<kind>` |
| `status` | `active` | active / complete / deferred / paused / captured |
| `revision` | `1` | Integer |
| `created` | `2026-06-25` | ISO date |
| `updated` | `2026-06-25` | ISO date |
| `product_area` | `Praxis / Public access` | Slash-separated context path |
| `supersedes` | prior object id | Or `none` |
| `superseded_by` | successor id | Or `none` |

## Object path rule

```
objects/<kind>/<human-title-slug>.md
```

Paths are human-readable current locators. Git preserves history.
Do not include dates, version numbers, or internal IDs in filenames.

## Staged term introductions

| Term | Introduced meaning | Current equivalent |
| --- | --- | --- |
| **Response** | Recorded reply to a Signal | (no current kind) |
| **Aim** | Outcome organized around under a Campaign | (no current kind) |
| **Stint** | Bounded movement: prepared, authorized, carried out, resolved | Fiber (current) |
| **Grant** | Authority-boundary object with explicit boundaries and validation | Directive (current) |
| **Resolution** | Closure layer after Execution | (no current kind) |