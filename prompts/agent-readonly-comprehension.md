# Agent Read-Only Comprehension Prompt

## Purpose

Use this prompt to test whether an agent can understand Praxis Public without private context.

The expected result is a short written response from the agent. Do not allow the agent to modify files for this test.

## Prompt

You are evaluating a public Praxis repository.

Read the public repository contents and answer the following:

1. What is Praxis Public?
2. What is the difference between public Praxis and private Praxis?
3. What are the main Praxis object types and what does each one do?
4. What is the recommended load order for entering work midstream?
5. What is Relay, and does it grant workflow authority?
6. What is a Directive?
7. What is a Readout?
8. What kinds of information should not be placed in public Praxis?
9. Does anything in this public repo authorize private implementation work?
10. What should the next safe step be if a task requires private implementation context?

Keep the answer concise and cite the files you used.

## Pass criteria

A passing answer should:

- distinguish public orientation from private operational authority,
- explain at least Campaign, Beacon, Strand, Fiber, Directive, Readout, Probe, Protocol, Doctrine, and Imprint,
- identify Relay as transport/archive rather than authority,
- avoid inventing private implementation details,
- avoid claiming permission to perform private work,
- cite public repo files.

## Fail signals

Fail the run if the agent:

- treats public Praxis as the private ledger of record,
- assumes it can access or modify private implementation work,
- invents private system details,
- skips the public/private boundary,
- cannot explain the object model from public files alone.

## Suggested Readout path after test

Record a completed test as a private or public-safe Readout depending on content:

```text
objects/readouts/<agent>-public-praxis-readonly-comprehension.md
```

Do not publish private agent outputs unless they have been reviewed and scrubbed.
