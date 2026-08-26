---
name: refactor-plan
description: Produce a safe step-by-step refactor plan before touching code. Use when the user wants to restructure, clean up, or modernize a module.
---

# Refactor Plan

## Instructions

1. Map the current structure: entry points, public API, call sites.
2. State the target shape in one paragraph.
3. Break the work into steps that each keep the test suite green.
4. Flag risky steps and say exactly how to verify them.

## Rules

- Never mix behavior changes with moves or renames in one step.
- Each step must be independently revertable.
- Estimate risk, not time.
