---
name: data-analysis
description: Use when analyzing actual experiment outputs, comparing methods across seeds or matched instances, selecting statistical tests, quantifying uncertainty and effect sizes, or checking the robustness of machine-learning and scheduling results.
---

# Data Analysis

Produce reproducible analysis from actual result files without inventing columns, measures, runs, or conclusions.

## Data inspection gate

List provided files; read exact schemas; identify the experimental unit, repeated-measure structure, seeds, instance identifiers, missing runs, and timeout rules; confirm which direction is better for every measure. Ask if a required interpretation is absent.

## Workflow

1. Validate completeness, duplicates, types, units, and configuration consistency.
2. Produce per-method descriptive summaries and uncertainty.
3. Determine whether comparisons are paired by instance, seed, or another recorded unit.
4. Select a test whose assumptions match the design.
5. Report effect size and confidence interval alongside significance results.
6. Handle multiple comparisons for a family of tests.
7. Separate exploratory findings from confirmatory claims.
8. Save analysis code and derived tables without modifying raw results.

Read references/review-prompts.md for the four-pass statistical review. Helpers are available through "python scripts/stat_summary.py --help" and "python scripts/format_pvalue.py --help". stat_summary.py requires NumPy and SciPy; report missing dependencies and do not install without authorization.

## Scheduling studies

Scheduling concepts may guide file inspection but never supply column names. Check whether outputs record objectives, arrival scenarios, instance identity, scale, runtime, feasibility, seed, and termination status. Compare matched instances whenever the recorded design permits it.

Do not assume makespan, flow time, tardiness, utilization, runtime, or any measure is present or optimized until established.

## Source

Adapted for Codex from lingzhi227/agent-research-skills, path skills/data-analysis/, inspected from the repository default branch on 2026-07-13.
