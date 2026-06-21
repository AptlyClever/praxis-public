# Praxis Public Solution

## Metadata

| Field | Value |
| --- | --- |
| id | `strand-praxis-public-solution` |
| type | `praxis.strand` |
| status | `active` |
| revision | `1-public` |
| created | `2026-06-20` |
| updated | `2026-06-20` |
| product_area | `Praxis / Public access / Agent workflow replacement` |
| source_scope | `public-safe curated summary` |
| supersedes | none |
| superseded_by | none |

## Purpose

Create a public-readable Praxis layer that lets humans and agents understand Praxis vocabulary, workflow shape, and evidence expectations without exposing private operational details.

## Problem

Private workflow context is fragile when agents cannot reliably search or load the private operational ledger.

If every agent evaluation depends on chat memory, exact private locators, or broad private repo access, then the evaluation measures context luck as much as agent quality.

A public Praxis layer gives agents a stable map before they receive any private task context.

## Design

Use a two-layer model:

| Layer | Role |
| --- | --- |
| Private Praxis | Operational ledger, full Directives, Records, Reports, runtime evidence, private implementation context |
| Public Praxis | Public-safe vocabulary, object model, scrubbed summaries, public examples, and agent comprehension prompts |

The public layer should be curated first, not automated first.

## Public-safe starter set

The initial seed should include:

- a public README,
- public/private boundary statement,
- object type translation map,
- sanitized Campaign summary,
- sanitized Strand summary,
- one public-safe Doctrine,
- one observation-only Probe,
- one read-only agent comprehension prompt.

## Pass criteria

The first public seed is useful when:

- the repo is public and readable,
- the starter set contains no private operational details,
- a human can understand the Praxis object model from the public repo alone,
- an agent can explain the public/private boundary,
- an agent can distinguish public orientation from private authority,
- an agent does not infer permission to merge, deploy, restart, access private repos, or operate systems.

## Non-goals

This Strand does not authorize:

- making private Praxis public,
- making implementation repos public,
- publishing private handoffs, reports, runtime logs, deployment details, LAN details, or security findings,
- using public Praxis as operational authority,
- replacing private Praxis as the ledger of record.

## Next movement

Seed the public surface, run read-only comprehension tests, then record real evaluation results as Readouts.
