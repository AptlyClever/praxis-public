# Mara Public Praxis Functional MVP Smoke

## Metadata

| Field | Value |
| --- | --- |
| id | `readout-mara-public-praxis-functional-mvp-smoke` |
| type | `praxis.readout` |
| status | `superseded` |
| result | `invalid-contaminated` |
| revision | `2-public` |
| created | `2026-06-25` |
| updated | `2026-06-25` |
| product_area | `Praxis / Public access / Functional MVP` |
| source_scope | `public-safe smoke result` |
| superseded_by | `readout-public-praxis-functional-mvp-independent-agent` |

## Purpose

Record and correct the first Mara / ChatGPT smoke test for the Praxis Public functional MVP startup path.

## Correction

This result must not count as MVP evidence.

The smoke test was performed inside the same ChatGPT conversation that helped design and create the Functional MVP artifacts. That means the test was context-contaminated: the model had access to conversation history and project framing beyond the public repo branch and startup prompt.

A contaminated test can show that the written files are internally coherent, but it cannot prove reliable public-context retrieval by a fresh agent.

## Prompt used

`prompts/agent-functional-mvp-startup.md`

## Files loaded

- `README.md`
- `FUNCTIONAL_MVP.md`
- `PUBLIC_PRIVATE_BOUNDARY.md`
- `prompts/agent-functional-mvp-startup.md`
- `objects/strands/praxis-direct-api-execution-harness.md`

## Original smoke answer summary

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

Invalid / contaminated.

The answer is plausible, but it is not independent evidence. It should not be used to claim functional MVP pass or partial-pass.

## Required replacement evidence

Run the same prompt in a clean agent context that receives only:

- the public repo branch,
- the startup prompt path,
- no private Praxis context,
- no prior chat history,
- no implementation repo context.

Record whether the independent agent loads public context reliably and keeps public orientation separate from private authority.

## Claude attempt note

A Claude attempt was started but did not complete because the service returned a temporary server-side rate-limit error after listing one directory. That is an infrastructure/tooling block, not a Praxis Public comprehension result.
