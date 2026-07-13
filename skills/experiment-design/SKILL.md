---
name: experiment-design
description: Use when planning machine-learning or algorithm experiments, especially early exploration, baseline comparisons, hyperparameter studies, multi-seed evaluation, ablations, sensitivity checks, or generalization tests.
---

# Experiment Design

Turn a confirmed research question into a staged, falsifiable, resource-aware experiment plan. Start with correctness and low-cost evidence.

## Required inputs

Read project files before using any identifier, dataset name, metric name, configuration key, or path. If an input is not established by files or the user, mark it unresolved and ask.

Capture the question, compared methods, controls, available instances, evaluation measures, resource limits, and current implementation state.

## Workflow

1. Correctness: define invariant checks, tiny deterministic cases, and a reproducible smoke run.
2. Baselines: verify each supplied baseline independently under matched conditions.
3. Focused exploration: vary one research dimension at a time; record expected observations and failure interpretation.
4. Robustness: run confirmed seeds, sensitivity checks, ablations, and out-of-setting tests when justified.
5. Decision: state what evidence advances, revises, or stops the direction.

For every run specify hypothesis, controls, changed variables, inputs, measures, seeds, budget, artifacts, completion criterion, and negative-result interpretation.

Read references/stage-prompts.md when a detailed four-stage plan is useful. Run "python scripts/design_experiments.py --help" for the generic scaffold. Treat generated grids only as scaffolds; replace values solely from inspected configuration or explicit choices.

## Dynamic job shop integration

When dynamic-job-shop-rl-research supplies context, separate simulator correctness, stochastic-arrival control, disjunctive-graph checks, supplied non-learning baselines, reinforcement-learning design studies, matched-instance evaluation, and generalization.

Do not select an arrival distribution, graph representation, action definition, reward, algorithm, objective, metric, instance scale, or seed count without evidence.

## Output

Return an experiment matrix, blocking unresolved questions, recommended first batch, stop/continue criteria, and exact artifacts to preserve.

## Source

Adapted for Codex from lingzhi227/agent-research-skills, path skills/experiment-design/, inspected from the repository default branch on 2026-07-13.
