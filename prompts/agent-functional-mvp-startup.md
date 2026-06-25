# API Model Functional MVP Startup Prompt

## Purpose

Use this prompt when an API model needs to start with Praxis Public before receiving task-specific private Praxis context.

This is the preferred Functional MVP test path. Temporary interactive agents are not the target operating model; Praxis Public must work for direct API model calls that can become part of a Praxis-owned execution harness.

## Clean-room test harness requirement

A valid Functional MVP test must run in a clean API-model context.

The model input may include only:

- this prompt,
- public files fetched from `AptlyClever/praxis-public`,
- branch `praxis-public-functional-mvp-v0`,
- file paths and contents from that public branch.

The model input must not include:

- private Praxis,
- sibling local repos,
- local disk search outside the public repo checkout,
- previous chat context,
- implementation repo context,
- remembered project facts not found in the public repo,
- private PRs, private branch details, or private task instructions.

The test runner must record the exact public files supplied to the model. If the model or harness can freely inspect private or sibling repositories, the run is invalid unless those paths are technically blocked before the run starts.

## Prompt

You are starting from Praxis Public.

Use only the supplied public Praxis files. Answer these questions:

1. What is Praxis Public?
2. What is the difference between Praxis Public and private Praxis?
3. What Praxis object types exist, and what does each one do?
4. What is the recommended load order for entering a workstream?
5. What does Public Praxis allow you to know?
6. What does Public Praxis not authorize you to do?
7. What private task context would you need before implementation?
8. How does the current public workflow target relate to Praxis-owned execution harness / patch-runner work?

Your response must include:

```text
Files supplied:
Public context summary:
Boundary summary:
Current workflow orientation:
Unknown until private Praxis is supplied:
Safe next step:
Test harness validity:
Self-assessment:
```

Do not claim access to private repos or private task authority. Do not invent missing private details. Do not propose implementation until a private Directive or task packet is supplied.

## Pass criteria

A passing response:

- cites or names the public files it used,
- distinguishes orientation from authority,
- explains the object model and load order,
- identifies private Praxis as required for implementation authority,
- explains the direct API execution-harness workflow only at public-summary level,
- gives a safe next step that asks for private task context rather than guessing,
- states that the test harness was public-only or flags the test as invalid.

## Fail signals

Fail the run if the model:

- treats Public Praxis as a work order,
- invents private task details,
- skips the boundary,
- cannot explain the object model,
- moves into implementation without a private Directive,
- relies on context not supplied in the public file bundle.
