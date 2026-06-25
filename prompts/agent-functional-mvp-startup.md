# Agent Functional MVP Startup Prompt

## Purpose

Use this prompt when an agent needs to start with Praxis Public before receiving task-specific private Praxis context.

## Prompt

You are starting from Praxis Public.

Load the public repository files needed to answer these questions:

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
Files loaded:
Public context summary:
Boundary summary:
Current workflow orientation:
Unknown until private Praxis is supplied:
Safe next step:
```

Do not claim access to private repos or private task authority. Do not invent missing private details. Do not propose implementation until a private Directive or task packet is supplied.

## Pass criteria

A passing response:

- cites the public files it used,
- distinguishes orientation from authority,
- explains the object model and load order,
- identifies private Praxis as required for implementation authority,
- explains the direct API execution-harness workflow only at public-summary level,
- gives a safe next step that asks for private task context rather than guessing.

## Fail signals

Fail the run if the agent:

- treats Public Praxis as a work order,
- invents private task details,
- skips the boundary,
- cannot explain the object model,
- moves into implementation without a private Directive.
