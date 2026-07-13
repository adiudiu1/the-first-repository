# Early Experiment Guide

Use this guide after the main Skill establishes which stage is active.

## Stage 1 gate: problem contract

Confirm from user statements or exact files:

- scheduling setting and operational constraints;
- dynamic events;
- arrival process, parameters, units, horizon, and reproducibility;
- optimization objective or objectives;
- disjunctive-graph node and edge semantics;
- graph feature and update definitions;
- MDP or environment contract;
- resource constraints;
- unresolved definitions.

Pass only when the behavior required by the next test is defined.

## Stage 2 gate: simulator correctness

Build the smallest tests supported by confirmed definitions:

- event chronology;
- job release visibility;
- operation precedence;
- machine exclusivity and capacity;
- processing start and completion;
- graph construction and dynamic update;
- feasible-action calculation;
- transition and termination;
- objective accumulation;
- repeatability under controlled randomness.

For every test record input, expected state transition, actual transition, and evidence location.

Pass only when blocking invariant failures are resolved.

## Stage 3 gate: baseline contract

For each established baseline record:

- exact source file and entry point;
- parameter source;
- observation or information access;
- decision timing;
- compute or decision budget;
- stopping condition;
- evaluation instances;
- structured result location.

Pass only when comparison conditions are interpretable.

## Stage 4 gate: minimal learning loop

Require:

- one verified environment configuration;
- confirmed state, action, reward, transition, and termination;
- confirmed algorithm and model configuration;
- controlled randomness;
- short training run;
- separate evaluation run;
- machine-readable results;
- logs and failure state;
- a defined success or diagnostic criterion.

Pass when the loop runs reproducibly and its outputs can be audited. Performance superiority is not required.

## Stage 5 gate: focused exploration

For each study write a one-row experiment contract:

- research question;
- hypothesis;
- one primary changed dimension;
- controls;
- instances;
- randomness;
- measures and improvement direction;
- budget;
- artifacts;
- completion rule;
- negative-result interpretation.

Prefer an experiment that separates two explanations over a wide search that only seeks a higher score.

## Stage 6 gate: robustness

Inspect the recorded design before choosing an analysis:

- experimental unit;
- matched-instance structure;
- seed structure;
- missing, failed, or timed-out runs;
- metric direction and units;
- distribution and variance;
- family of comparisons;
- generalization boundary.

Report uncertainty and effect size. Choose statistical tests only after the structure is established.

## Stage 7 gate: preserve state

Store confirmed state using exact existing schemas. The research memory should make these answerable in a new conversation:

- What question is being tested?
- Which definitions are locked?
- Which implementation is current?
- Which experiments ran?
- Where are results?
- What failed?
- What decision followed?
- What remains unresolved?
- What is the next smallest action?

## Stop conditions

Stop and ask one precise question when:

- two sources conflict;
- a required definition is missing;
- a requested command or path cannot be found;
- the comparison would be unfair or uninterpretable;
- the simulator violates a confirmed invariant;
- the result schema cannot identify the experimental unit;
- continuing would overwrite human research decisions or raw evidence.

