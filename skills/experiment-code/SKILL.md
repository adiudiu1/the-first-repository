---
name: experiment-code
description: Use when implementing, debugging, or improving reproducible machine-learning and algorithm experiments from an approved experiment plan, including simulators, environments, training, evaluation, logging, and result plots.
---

# Experiment Code

Implement the smallest reproducible experiment slice that tests one approved claim. Preserve the existing repository structure and exact identifiers.

## Inspection gate

Before editing, read repository instructions and the experiment plan; locate exact entry points, configurations, data schemas, result formats, tests, and dependencies; then run the smallest existing verification.

Ask when a required path, key, class, function, metric, or schema cannot be found. Never impose a framework, layout, naming convention, or command when project files establish something else.

## Boundaries

Keep instance and event generation, simulator transition and feasibility, environment interface, algorithm, configuration and seeding, evaluation, logging, checkpoints, and plotting separable.

Implement one vertical slice first: fixed input, deterministic seed, short run, machine-readable output, and an assertion for the expected invariant.

## Workflow

For generation, map planned runs to exact configuration changes, add tests before behavior, follow the existing output schema, and avoid placeholders.

For debugging, reproduce the exact failure, identify the first incorrect state or violated invariant, make the smallest fix, and rerun the reproduction plus relevant tests.

For improvement, compare with preserved prior results, change one justified factor, retain negative outcomes, and do not tune on final evaluation instances.

Read references/experiment-prompts.md and references/code-patterns.md only after repository inspection. Translate Claude-specific examples conceptually; never use their absolute paths.

## Dynamic job shop integration

Require tests for every confirmed invariant involving event order, arrival, precedence, capacity, graph updates, feasible actions, terminal conditions, and objective accumulation. Exact invariant definitions must come from project files or the user.

## Source

Adapted for Codex from lingzhi227/agent-research-skills, path skills/experiment-code/, inspected from the repository default branch on 2026-07-13.
