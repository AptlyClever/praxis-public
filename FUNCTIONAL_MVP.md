# Praxis Public Functional MVP

Praxis Public is the public-readable orientation layer for Praxis.

It exists so an agent or API model can load stable workflow vocabulary, object model, evidence expectations, and public-safe current-work orientation before receiving private task context.

## What Praxis Public is

Praxis Public is:

- a public orientation surface for humans, ChatGPT, and API models,
- a stable reference for Praxis object types and load order,
- a public-safe map of selected Control Alt workflow lanes,
- a context-retrieval target for startup prompts,
- a test corpus for comprehension and workflow-readiness checks,
- a bridge from general workflow understanding to private Praxis authority.

## What Praxis Public is not

Praxis Public is not:

- the private Praxis ledger,
- a place for private task details,
- permission to modify implementation repositories,
- permission to perform operational work,
- a replacement for private Directives, Reports, or Readouts,
- a substitute for operator authorization.

## How it works

Praxis uses a two-layer context model:

| Layer | Role |
| --- | --- |
| Praxis Public | Public orientation: vocabulary, object model, scrubbed summaries, prompts, and safe examples |
| Private Praxis | Operational authority: full task context, Directives, reports, implementation evidence, and private decisions |

A fresh agent, ChatGPT conversation, or API model should load Praxis Public first to understand how Praxis works. Then it must receive a private Directive or task packet before doing private implementation work.

Public Praxis can answer: "How should I think about this workflow?"

Private Praxis answers: "What am I authorized to do right now?"

## Functional MVP criteria

Praxis Public reaches functional MVP when it can do all of the following:

1. Clearly define Praxis Public and its relationship to private Praxis.
2. Let both a clean API model call and a clean ChatGPT conversation retrieve context reliably using public startup prompts.
3. Maintain a safe reviewed link from private Praxis source objects to public Praxis target artifacts.
4. Help in a real current workflow with recorded evidence.

Seed docs and standalone comprehension tests are not enough. The public layer must be useful in an actual workflow path, and it must work for ChatGPT too.

## Required MVP tests

Functional MVP requires both tests:

1. **API model clean-room test** — a direct API model receives only the prompt and public file bundle.
2. **ChatGPT clean-room test** — a new ChatGPT conversation receives only the public repo branch and clean-room prompt.

Either test may fail or return partial; the result must be recorded honestly. The MVP is not a pass unless both tests show that Praxis Public can orient the model without leaking into private authority or invented context.

## Current MVP workflow target

The current workflow target is Praxis-owned direct API execution harness / patch-runner work.

Praxis Public should orient an agent to this goal:

- Control Alt is reducing dependence on any single build / execution agent.
- The intended direction is a Praxis-owned execution harness using direct API providers under explicit boundaries.
- Public Praxis provides the shared map and vocabulary.
- Private Praxis still supplies the Directive, allowed paths, validation requirements, and evidence destination.

This public summary does not authorize building the runner. It only orients agents before private task authority is supplied.
