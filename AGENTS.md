# AGENTS.md

Agent orientation for Praxis Public.

## What you have access to

- `README.md` — Praxis object model and lifecycle
- `OBJECT_MODEL.md` — Full object kind definitions and metadata schema
- `PUBLIC_PRIVATE_BOUNDARY.md` — Public-safe vs private-only boundary
- `CURRENT_WORK.md` / `CURRENT_WORK.json` — Active work summary with purpose statements
- `HISTORY_INDEX.md` — Index of completed work
- `AGENTS.md` — This file
- `prompts/agent-startup.md` — Recommended startup prompt
- `public-index.json` — Machine-readable index of all objects with summaries
- `public-index-summary.json` — Compact public-safe counts
- `FRESHNESS.md` / `FRESHNESS.json` — Generation timestamp and source info
- `objects/` — Public-safe Praxis object copies

## What you do NOT have access to

- Private Praxis (full handoffs, runtime reports, deploy/device/network details)
- Private implementation repos or local disk state
- Implementation authority — you cannot deploy or apply from public context

## How to orient yourself

1. Load `README.md` for the object model and lifecycle.
2. Load `PUBLIC_PRIVATE_BOUNDARY.md` for the public/private split.
3. Load `CURRENT_WORK.md` for active work context with purpose summaries.
4. Follow `prompts/agent-startup.md`.

## When you need private context

1. State clearly that you need a private Directive or private task context.
2. Do not infer private details from Public Praxis alone.
3. Do not propose implementation without a private Directive.
4. Ask the operator to supply the relevant private Praxis objects or task packet.

## Object count summary

- **Beacons**: 2 total (2 active, 0 complete)
- **Campaigns**: 1 total (1 active, 0 complete)
- **Directives**: 51 total (9 active, 40 complete)
- **Doctrines**: 18 total (11 active, 0 complete)
- **Fibers**: 51 total (8 active, 42 complete)
- **Imprints**: 24 total (7 active, 0 complete)
- **Probes**: 8 total (0 active, 1 complete)
- **Protocols**: 7 total (3 active, 0 complete)
- **Readouts**: 68 total (0 active, 63 complete)
- **Signals**: 18 total (15 active, 0 complete)
- **Strands**: 5 total (2 active, 1 complete)