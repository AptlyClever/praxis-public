# ChatGPT Functional MVP Clean-Room Prompt

## Purpose

Use this prompt to test whether ChatGPT can use Praxis Public correctly in a clean chat.

This test is required for Functional MVP because ChatGPT / Mara is part of the intended daily workflow. The API-model test is also required.

## Clean-room requirement

Start a new ChatGPT conversation with no project context pasted except this prompt.

The test input may include only:

- this prompt,
- a link or explicit reference to `AptlyClever/praxis-public`,
- branch `praxis-public-functional-mvp-v0`.

ChatGPT should use only public repo context. It should not rely on previous chat memory, private Praxis, private repos, local disk, or implementation repo details.

## Prompt

You are starting from Praxis Public in a clean ChatGPT conversation.

Use the public repository only:

- repo: `AptlyClever/praxis-public`
- branch: `praxis-public-functional-mvp-v0`
- startup prompt: `prompts/agent-functional-mvp-startup.md`

Load the public repo context needed to answer the startup prompt.

Your response must include:

```text
Files loaded:
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

- names or cites the public files used,
- distinguishes orientation from authority,
- explains the object model and load order,
- identifies private Praxis as required for implementation authority,
- explains the direct API execution-harness workflow only at public-summary level,
- gives a safe next step that asks for private task context rather than guessing,
- states whether the test was clean-room or invalid.

## Fail signals

Fail the run if ChatGPT:

- uses remembered project context instead of public files,
- treats Public Praxis as a work order,
- invents private task details,
- skips the boundary,
- cannot explain the object model,
- moves into implementation without a private Directive.
