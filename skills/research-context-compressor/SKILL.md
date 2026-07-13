---
name: research-context-compressor
description: Use when a research project must preserve its confirmed question, repository orientation, experiments, datasets, decisions, run history, and open questions so later conversations can continue without rescanning the entire project.
---

# Research Context Compressor

Maintain compact project memory under .research/ from inspected evidence. Empty fields are better than invented content.

## Inputs

Read existing .research/ files, root instructions, README.md, dependency and configuration files, exact experiment entry points, documented data and output directories, and recent Git history when available.

List large directories before selecting representative files. Do not rescan the whole repository when manifests establish the information.

## Outputs

Write project_manifest.yml, conditional experiment_matrix.yml and data_dictionary.yml, run_log.md, decisions.md, and open_questions.md under the exact .research/ directory.

Read references/research-workspace-manifest.md for schemas. references/example-humanities-project.md illustrates that missing information stays empty.

## Update rules

Update rather than replace human edits. Ask before changing conflicting provenance or a locked decision. Preserve exact established keys. Record unknown values in open_questions.md. Never infer a question, hypothesis, claim, dataset schema, result, or stage. Do not alter raw data or experiment outputs.

## Dynamic job shop integration

When confirmed, record the problem setting, stochastic-arrival specification, disjunctive graph, MDP, simulator entry points, baseline implementations, configurations, result locations, and unresolved choices. Do not create definitions from convention.

## Source

Adapted for Codex from WenyuChiou/research-hub, path skills/research-context-compressor/, plus docs/research-workspace-manifest.md, inspected from branch master on 2026-07-13.
