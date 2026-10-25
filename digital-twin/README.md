# Digital twin and scenario modeling

The intended product lets people watch a regional homestead develop, inspect why outcomes change, and follow hypothetical households over decades. This directory currently contains a specification and research plan, not a new simulation implementation.

Work as a simulation engineer and systems modeler, using the [model contract](MODEL-CONTRACT.md) and [scenario plan](SCENARIO-PLAN.md). Research departments supply evidence, costs, constraints, and uncertainty. The model must preserve those limits instead of supplying favorable missing values.

## Build toward the experience in stages

1. Reconcile the existing prototype with the current vision and identify its assumptions.
2. Establish a transparent entity-based financial and resource model for a bounded first-node case.
3. Calibrate the parts with available observations and compare them with simpler benchmarks.
4. Add heterogeneous synthetic households, decisions, entry and exit, and alternative growth paths.
5. Connect the model to an explanatory bird's-eye landscape, time controls, household stories, and scenario comparison.

Each stage needs separate scope and validation. A century-scale view should expose uncertainty and regime changes rather than imply century-scale predictive accuracy. [Site integration](../site/README.md) records the existing prototype separately.
