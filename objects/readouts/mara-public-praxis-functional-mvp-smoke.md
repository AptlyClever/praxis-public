# Mara Public Praxis Functional MVP Smoke

## Metadata

| Field | Value |
| --- | --- |
| id | `readout-mara-public-praxis-functional-mvp-smoke` |
| type | `praxis.readout` |
| status | `complete` |
| result | `partial-pass` |
| revision | `1-public` |
| created | `2026-06-25` |
| updated | `2026-06-25` |
| product_area | `Praxis / Public access / Functional MVP` |
| source_scope | `public-safe smoke result` |

## Purpose

Record a public-safe smoke test for the Praxis Public functional MVP startup path.

This is not final MVP certification. It is evidence that the new public files can orient an agent toward the current workflow target while preserving the public/private boundary.

## Prompt used

`prompts/agent-functional-mvp-startup.md`

## Files loaded

- `README.md`
- `FUNCTIONAL_MVP.md`
- `PUBLIC_PRIVATE_BOUNDARY.md`
- `prompts/agent-functional-mvp-startup.md`
- `objects/strands/praxis-direct-api-execution-harness.md`

## Smoke answer summary

Public context summary:

Praxis Public is the public-readable orientation layer for Praxis. It gives agents stable vocabulary, object model, evidence expectations, and public-safe workflow orientation before private task context is supplied.

Boundary summary:

Public Praxis provides orientation only. Private Praxis remains the authority layer for Directives, task-specific context, implementation boundaries, validation requirements, and evidence destination.

Current workflow orientation:

The current MVP workflow target is the Praxis-owned direct API execution harness / patch-runner. Public Praxis can explain why this lane exists and what kind of evidence Praxis expects, but it cannot authorize implementation.

Unknown until private Praxis is supplied:

- exact private Directive,
- task-specific boundaries,
- validation expectations,
- evidence destination,
- whether implementation is authorized.

Safe next step:

Request or load the private Praxis Directive and task packet before proposing or performing implementation.

## Result

Partial pass.

The public startup path can orient an agent toward the correct workflow and boundary. This run is only a Mara / ChatGPT smoke test; it still needs an independent agent run before claiming full functional MVP pass.

## Follow-up required

- Run the same prompt with at least one independent implementation-capable agent.
- Record whether it loads the public context reliably.
- Record whether it keeps public orientation separate from private authority.
