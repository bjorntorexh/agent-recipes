---
name: test-writer
description: Write focused unit tests for a module or function. Use when the user asks to add tests, improve coverage, or make a module testable.
---

# Test Writer

## Instructions

1. Read the module first; list its public surface.
2. Write tests for behavior, not implementation details.
3. Cover: happy path, boundary values, error cases.
4. Use fixtures and temp dirs; never touch the network or real FS state.
5. Name tests as test_<unit>_<scenario>_<expectation>.

## Rules

- One assertion theme per test.
- No sleeps; use fakes for time.
- If the code is untestable, say why and propose the smallest refactor.
