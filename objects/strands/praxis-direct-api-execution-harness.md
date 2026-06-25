# Praxis Direct API Execution Harness

## Metadata

| Field | Value |
| --- | --- |
| id | `strand-praxis-direct-api-execution-harness` |
| type | `praxis.strand` |
| status | `public-summary` |
| revision | `1-public` |
| created | `2026-06-25` |
| updated | `2026-06-25` |
| product_area | `Praxis / Execution harness / Agent workflow replacement` |
| source_scope | `public-safe summary` |

## Purpose

This public summary orients agents to the current workflow direction: Control Alt is moving toward a Praxis-owned execution harness that can use direct API providers under Praxis authority.

## Public summary

The goal is not to replace one paid agent wrapper with another. The goal is a Praxis-owned workflow where:

- Praxis supplies context and authority boundaries,
- a bounded runner can request model assistance through provider APIs,
- outputs are structured as patch proposals, validation results, usage records, and Readouts,
- private Praxis remains the operational ledger,
- humans keep final authorization over implementation and merge decisions.

## Relationship to Praxis Public

Praxis Public should let a fresh agent understand this workflow direction before private task context is supplied.

Praxis Public can explain:

- why an execution harness exists,
- what kind of evidence Praxis expects,
- why public context is orientation only,
- why private Directives are still required before implementation.

Praxis Public cannot authorize the runner to modify code, call providers, or operate private systems.

## Functional MVP test use

This Strand summary is the preferred real-workflow target for Praxis Public functional MVP testing.

A passing agent should be able to say:

1. The current workflow direction is Praxis-owned direct API execution.
2. Public Praxis provides orientation and shared vocabulary.
3. Private Praxis must provide the specific Directive, allowed paths, validation expectations, and evidence destination.
4. The agent must not implement anything from this public summary alone.

## Boundary

This public summary intentionally omits private implementation details. It is a map, not a work order.
